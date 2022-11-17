# Solidity

Официальная документация: [https://solidity.readthedocs.io/en/latest/introduction-to-smart-contracts.html](https://solidity.readthedocs.io/en/latest/introduction-to-smart-contracts.html)\
Security Recomendations: [https://solidity.readthedocs.io/en/latest/security-considerations.html](https://solidity.readthedocs.io/en/latest/security-considerations.html)

Solidity Langs: [https://soliditylang.org/](https://soliditylang.org/)

Особенности языка

перевести string в bytes32 - это просто перевести в hex!

фишки:\
какие-то важные вещи могут хранится в коде контракта\
какие-то важные вещи могут палиться при ошибках (например: отправляем в функцию неверные данные, контракт отрабатывает с ошибкой, мы в транзакции смотрим ошибку -> палим какой-нибудь аргумент)

Норм статьи: \
[https://medium.com/coinmonks/a-practical-walkthrough-smart-contract-storage-d3383360ea1b](https://medium.com/coinmonks/a-practical-walkthrough-smart-contract-storage-d3383360ea1b)\
[https://programtheblockchain.com/posts/2018/03/09/understanding-ethereum-smart-contract-storage/](https://programtheblockchain.com/posts/2018/03/09/understanding-ethereum-smart-contract-storage/)

reentrancy attack: [https://medium.com/@gus\_tavo\_guim/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4](https://medium.com/@gus\_tavo\_guim/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4)\


