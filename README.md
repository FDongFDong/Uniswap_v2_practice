# DeFi App Based on Uniswap v2

Simple decentralized application based on Solidity and Web3 that swap a simple pair of tokens with the help of the Uniswap V2 library.

## Technology Stack & Tools

- Solidity (Writing Smart Contract)
- Javascript (React & Testing)
- [Web3](https://web3js.readthedocs.io/en/v1.5.2/) (Blockchain Interaction)
- [Truffle](https://www.trufflesuite.com/docs/truffle/overview) (Development Framework)
- [Ganache CLI](https://github.com/trufflesuite/ganache-cli-archive) (For Local Blockchain)
- [Infura](https://infura.io/) (Ethereum Node As A Service Provider)

## Requirements For Initial Setup

- Install [NodeJS](https://nodejs.org/en/), should work with any node version below 16.5.0
- Install [Truffle](https://www.trufflesuite.com/docs/truffle/overview), In your terminal, you can check to see if you have truffle by running `truffle version`. To install truffle go to your project root directory and run `npm install --save-dev truffle` Ideal to have truffle version 5.4 to avoid dependency issues.
- Install [Ganache CLI](https://github.com/trufflesuite/ganache-cli-archive).

## Setting Up

### 1. Clone/Download the Repository

```
$ git clone https://github.com/davdotsol/uniswap-v2-defi-app.git
$ cd uniswap-v2-defi-app
$ git checkout starter
```

### 2. Install Dependencies:

```
$ cd uniswap-v2-defi-app
$ npm install
```

### 3. Start Ganache

`$ npm run ganache`

### 4. Start React
`$ npm run start`

### 5. Migrate Smart Contracts

`$ npx truffle migrate --reset --skip-dry-run`

### Troubleshooting
- truffle 버전을 확인해주세요
-- trffle 배포가 안되면 src/abis 파일을 날리고 재배포 해주세요
-- 그래도 안되면 앞에 sudo를 입력하고 해주세요
-- 그래도 안되면 sudo rm -rf ~/Library/Preferences/truffle-nodejs 해당 파일을 삭제 후 package-json에 있는 truffle을 재설치 해주세요

- ganache network를 사용하기 때문에 ganache가 먼저 켜져있어야 합니다.
-- ganache 첫번째 계정 사용 - 메타마스크에서 가나슈 네트워크 생성 후 비밀키를 이용해 가나슈 계정 불러오기 -- 비밀키는 App.js에서 console에 찍어줌

- 메타마스크에서 이더리움 전송 시 RPC Error가 뜨면 계정을 초기화해주세요
-- https://ethereum.stackexchange.com/questions/30921/tx-doesnt-have-the-correct-nonce-metamask
