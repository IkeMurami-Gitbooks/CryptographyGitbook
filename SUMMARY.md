# Table of contents

* [Crypto Book](README.md)
  * [People and Blogs](master/people-and-blogs.md)

## Симметричное шифрование

* [Блочные шифры](simmetrichnoe-shifrovanie/blochnye-shifry/README.md)
  * [AES](simmetrichnoe-shifrovanie/blochnye-shifry/aes/README.md)
    * [Атаки](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/README.md)
      * [AES-ECB: Padding Oracle Attacks](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/aes-ecb-padding-oracle-attacks.md)
      * [AES-CBC: Bitflip](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/backflip.md)
      * [AES-CBC: Padding Oracle](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/aes-cbc-padding-oracle.md)
      * [AES-CTR: Fixed nonce](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/aes-ctr-fixed-nonce.md)
      * [AES-CTR: Bitflip](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/aes-ctr-bitflip.md)
      * [AES-CBC: Key=IV insecure](simmetrichnoe-shifrovanie/blochnye-shifry/aes/ataki/aes-cbc-key-iv-insecure.md)
  * [DES](simmetrichnoe-shifrovanie/blochnye-shifry/des.md)
* [Поточные шифры](simmetrichnoe-shifrovanie/untitled/README.md)
  * [Корреляционный анализ](simmetrichnoe-shifrovanie/untitled/korrelyacionnyi-analiz.md)
  * [Алгоритм Берлекэмпа-Месси восстановления внутреннего состояния ЛРС по гамме](simmetrichnoe-shifrovanie/untitled/algoritm-berlekempa-messi-vosstanovleniya-vnutrennego-sostoyaniya-lrs-po-gamme.md)
* [RNG](simmetrichnoe-shifrovanie/rng/README.md)
  * [Mersenne Twister RNG](simmetrichnoe-shifrovanie/rng/mersenne-twister-rng.md)

## Асимметричное шифрование

* [Эллиптические кривые](asimmetrichnoe-shifrovanie/ellipticheskie-krivye.md)
* [Tools](asimmetrichnoe-shifrovanie/tools/README.md)
  * [Факторизация чисел](asimmetrichnoe-shifrovanie/tools/faktorizaciya-chisel.md)
  * [RSATool](asimmetrichnoe-shifrovanie/tools/rsatool.md)
* [Diffie-Hellman](asimmetrichnoe-shifrovanie/diffie-hellman.md)
* [Атаки на RSA](asimmetrichnoe-shifrovanie/ataki-na-rsa/README.md)
  * [Вычисление квадратного корня по модулю](asimmetrichnoe-shifrovanie/ataki-na-rsa/vychislenie-kvadratnogo-kornya-po-modulyu.md)
  * [Если известна часть закрытой экспоненты или экспонента мала (e=3)](asimmetrichnoe-shifrovanie/ataki-na-rsa/esli-izvestna-chast-zakrytoi-eksponenty.md)
  * [Базовые атаки](asimmetrichnoe-shifrovanie/ataki-na-rsa/bazovye-ataki.md)
* [Статьи](asimmetrichnoe-shifrovanie/stati.md)

## Классические шифры

* [Enigma](klassicheskie-shifry/enigma.md)
* [Tools](klassicheskie-shifry/untitled/README.md)
  * [playfair brecker](klassicheskie-shifry/untitled/playfair-brecker.md)
  * [Атаки на классические шифры](klassicheskie-shifry/untitled/ataki-na-klassicheskie-shifry.md)
  * [Поиск слов по шаблону](klassicheskie-shifry/untitled/poisk-slov-po-shablonu.md)

## Хеш-функции

* [MAC](khesh-funkcii/mac/README.md)
  * [Attacks](khesh-funkcii/mac/attacks/README.md)
    * [SHA1-MAC: Length-Extension Attack](khesh-funkcii/mac/attacks/sha1-mac-length-extension-attack.md)
    * [HMAC-SHA1: Break with an artificial timing leak — утечки времени](khesh-funkcii/mac/attacks/hmac-sha1-break-with-an-artificial-timing-leak-utechki-vremeni.md)
* [KDF](khesh-funkcii/kdf.md)
* [Tools](khesh-funkcii/untitled.md)

## Блокчейн-технологии

* [Script](blokchein-tekhnologii/untitled.md)
* [Web3](blokchein-tekhnologii/web3.md)
* [DeFi](blokchein-tekhnologii/defi.md)
* [ZK | Zero Knowledge](blokchein-tekhnologii/zk.md)
* [Etherium Blockchain Contracts](blokchein-tekhnologii/etherium-blockchain-contracts/README.md)
  * [About Smart-contracts and Ethereum](blokchein-tekhnologii/etherium-blockchain-contracts/o-smart-kontraktakh-i-ethereum.md)
  * [ERC](blokchein-tekhnologii/etherium-blockchain-contracts/erc.md)
  * [EVM | Ethereum Virtual Machine](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/README.md)
    * [Concepts](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/concepts.md)
    * [Languages](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/languages/README.md)
      * [Solidity](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/languages/solidity.md)
      * [Yul](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/languages/yul.md)
      * [Viper](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/languages/viper.md)
      * [Rust](blokchein-tekhnologii/etherium-blockchain-contracts/evm-or-ethereum-virtual-machine/languages/rust.md)
  * [Development Platforms And Frameworks](blokchein-tekhnologii/etherium-blockchain-contracts/development-platforms-and-frameworks/README.md)
    * [Truffle](blokchein-tekhnologii/etherium-blockchain-contracts/development-platforms-and-frameworks/truffle.md)
    * [Hardhat](blokchein-tekhnologii/etherium-blockchain-contracts/development-platforms-and-frameworks/hardhat.md)
    * [Brownie](blokchein-tekhnologii/etherium-blockchain-contracts/development-platforms-and-frameworks/brownie.md)
    * [Remix IDE](blokchein-tekhnologii/etherium-blockchain-contracts/development-platforms-and-frameworks/solidity-ide.md)
  * [Настройка окружения (на базе Remix IDE)](blokchein-tekhnologii/etherium-blockchain-contracts/nastroika-okruzheniya.md)
  * [Blockchain Platforms](blokchein-tekhnologii/etherium-blockchain-contracts/blockchain-platforms.md)
  * [OpenZeppelin](blokchein-tekhnologii/etherium-blockchain-contracts/openzeppelin.md)
  * [CTF examples](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/README.md)
    * [HoneyPots](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/honeypots.md)
    * [Sharkyctf2020](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/sharkyctf2020.md)
    * [PHDays10](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/phdays10.md)
    * [OpenZeppelin Ethernaut](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/openzeppelin-ethernaut.md)
    * [List of CTFs](blokchein-tekhnologii/etherium-blockchain-contracts/ctf-examples/list-of-ctfs.md)
  * [Talks & Papers](blokchein-tekhnologii/etherium-blockchain-contracts/talks-and-papers.md)
  * [Tools](blokchein-tekhnologii/etherium-blockchain-contracts/tools.md)
  * [Vulnerabilities](blokchein-tekhnologii/etherium-blockchain-contracts/vulnerabilities.md)
  * [Companies](blokchein-tekhnologii/etherium-blockchain-contracts/company.md)
* [API некоторых валют](blokchein-tekhnologii/api-nekotorykh-valyut.md)
* [Hyperledger](blokchein-tekhnologii/hyperledger.md)
* [Tools](blokchein-tekhnologii/tools.md)
* [Mixers](blokchein-tekhnologii/mixers.md)

## Прикладное шифрование

* [Свой SSL Cert для сайта](prikladnoe-shifrovanie/svoi-ssl-cert-dlya-saita.md)
* [How Certificate Transparency Works](prikladnoe-shifrovanie/how-certificate-transparency-works.md)
* [DPAPI](prikladnoe-shifrovanie/dpapi.md)
* [OpenSSL](prikladnoe-shifrovanie/openssl/README.md)
  * [Чтение сертификатов и ключей](prikladnoe-shifrovanie/openssl/chtenie-sertifikatov-i-klyuchei.md)

## Learning

* [Certificates](learning/certificates.md)
* [Books & Papers](learning/books-and-papers.md)
