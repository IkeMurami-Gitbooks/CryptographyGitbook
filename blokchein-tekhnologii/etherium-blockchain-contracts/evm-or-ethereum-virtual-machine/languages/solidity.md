# Solidity

Официальная документация: [https://solidity.readthedocs.io/en/latest/introduction-to-smart-contracts.html](https://solidity.readthedocs.io/en/latest/introduction-to-smart-contracts.html)\
Security Recomendations: [https://solidity.readthedocs.io/en/latest/security-considerations.html](https://solidity.readthedocs.io/en/latest/security-considerations.html)

Solidity Langs: [https://soliditylang.org/](https://soliditylang.org/)

Интерактивная платорма для обучения программированию на Solidity: [https://cryptozombies.io/en/course](https://cryptozombies.io/en/course)

Особенности языка

перевести string в bytes32 - это просто перевести в hex!

фишки:\
какие-то важные вещи могут хранится в коде контракта\
какие-то важные вещи могут палиться при ошибках (например: отправляем в функцию неверные данные, контракт отрабатывает с ошибкой, мы в транзакции смотрим ошибку -> палим какой-нибудь аргумент)

Норм статьи: \
[https://medium.com/coinmonks/a-practical-walkthrough-smart-contract-storage-d3383360ea1b](https://medium.com/coinmonks/a-practical-walkthrough-smart-contract-storage-d3383360ea1b)\
[https://programtheblockchain.com/posts/2018/03/09/understanding-ethereum-smart-contract-storage/](https://programtheblockchain.com/posts/2018/03/09/understanding-ethereum-smart-contract-storage/)

reentrancy attack: [https://medium.com/@gus\_tavo\_guim/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4](https://medium.com/@gus_tavo_guim/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4)\


Solidity Semgrep Pack: [https://www.linkedin.com/posts/decurity\_were-glad-to-announce-that-our-grant-proposal-activity-7044578630047272960-GwsO?utm\_source=share\&utm\_medium=member\_ios](https://www.linkedin.com/posts/decurity_were-glad-to-announce-that-our-grant-proposal-activity-7044578630047272960-GwsO?utm_source=share\&utm_medium=member_ios)

## Декомпиляторы

https://ethervm.io/decompile - онлайн-декомпилятор solidity

https://contract-library.com/ - библиотека контрактов с исходниками и декомпилятором

https://eveem.org/ - декомпиляция в псевдокод, похожий на Python

