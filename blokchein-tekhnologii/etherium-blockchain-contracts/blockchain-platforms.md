# Blockchain Platforms

Для запуска своих смарт-контрактов необходимо подключиться к blockchain-платформе. Это может быть Ethereum blockchain (наз "mainnet" или "main network") — требует реальных денег. Можно использовать тестовые сети — Ropsten, Rinkeby, Kovan и Goerli. Однако, для запуска автотестов они не очень подходят по той причине, что транзакации будут требовать время на подтверждение. Третий вариант — использовать local blockchain. В этом случае сеть поднимается локально и все операции выполняются мгновенно.

## Local Blockchain

[Ganache](https://github.com/trufflesuite/ganache-cli) — одна из популярных local blockchain platform

```
Add to your project:

$ npm install --save-dev ganache-cli



При запуске Ganache создаст случайный набор разблокированных учетных записей 
и предоставит им эфир. Чтобы получить те же адреса, которые будут использоваться 
в этом руководстве, вы можете запустить Ganache в детерминированном режиме:

$ npx ganache-cli --deterministic
```

**Truffle** has a graphical version of `ganache-cli`, also called [Ganache](https://www.trufflesuite.com/ganache).

## Near

Near Blockchain Protocol: [https://near.org/](https://near.org/)

## Solana

Solana Blockchain Platform: [https://solana.com/ru](https://solana.com/ru)

Эта платформа переживает проблемы после краха FTX (Solana продвигался основателем FTX): финансовые последствия — падение токена SOL, нефинансовые — отток разработчиков (несколько крупных проектов заявили о переносе на Etherium и Polygon)

## Polygon

От Polygon Technology



## Platforms Based on Rust

Не мало платформ базируются на Rust. Например, Solana.

Link: [https://www.itmagination.com/blog/rust-development-blockchain-web3](https://www.itmagination.com/blog/rust-development-blockchain-web3)

## Кошельки (работа с аккаунтом/аккаунтами) для разработки

### MetaMask

### Influro

### Alchemy

## Другие проекты

Пока не знаю, к чему они ближе

* Aztec
* Aleo
* Nethermind
* Polygon
* Mach 34: [https://mach34.space/](https://mach34.space/)
* CipherTrace: [https://ciphertrace.com/](https://ciphertrace.com/)
