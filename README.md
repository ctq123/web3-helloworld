# web3-helloworld

编写第一个web3智能合约，基于truffle框架

## 1. 安装

```bash
npm install -g truffle
npm install -g ganache-cli
```

> 版本说明
> truffle@6.14.13 ganache-cli@6.14.13 node@16.14.0

## 2. 启动 Ganache

新建一个终端terminal窗口执行命令
```bash
ganache-cli
```

## 3 部署合约

新建另一个终端terminal窗口执行命令
```bash
truffle migrate
```

## 4. 验证

使用 Truffle 控制台与合约互动
```bash
truffle console
```

## 5. 互动

在控制台中执行以下命令：
```js
const hello = await HelloWorld.deployed();
let greeting = await hello.getGreeting();
console.log(greeting); // 输出 "Hello, World!"
await hello.setGreeting("Hello, Blockchain!");
greeting = await hello.getGreeting();
console.log(greeting); // 输出 "Hello, Blockchain!"
```
