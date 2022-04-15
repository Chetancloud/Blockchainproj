# Project Title

* ERC20 Smart Contract Deployment and Token Distribution on Ropsten Network

## Description

*This project demonstrates the methodology to modify ERC20 smart contract deployment in a way which enables it to create a node js application that distributes the equal number of tokens on multiple Metamask accounts at once.This report will also explain how to use docker for for node js application so that this application can be run from any operating system platform
## Getting Started

### prerequisites

* 10 metamask addresses , Github versioning control setup, Infura Token , Remix IDE , Linux terminal to run node js application.

### Installing
* 1.Git clone
 ```
git clone https://github.com/agrawallalit/NCI_Blockchain
```
*2. Modify DeployedContract.sol as per below (you can change contract name , _name and _symbol values as you wish)
```
line:146 : contract X21166374ERC20 is Context, IERC20, IERC20Metadata{ ..
```
```
line:166 : _name = "X21166374TOKEN";
          _symbol = "MSCloud";
```

### Compile and then deploy X21166374ERC20 contract on Remix IDE 

* Modify .env file for actual values please refer .env file form above repository.
```
INFURA_TOKEN= < Infura Project Token >
CONTRACT_ADDRESS= < Address of Contract deployed>
OWNER_ADDRESS= < Metamask Account ID >
PRIVATE_KEY= < Private from Metamask Account >
```

### Open Linux terminal

### install for envionment dependencies using NPM (Node Package Manager) as follow.
```
npm i fs big-number dotenv ethereumjs-tx web3

```

### Remove node_modules as below cmd
```
\rm node_modules
```
### Reinstall node_modules as below
```
npm i
```
### Now run distribute.js as per below cmd and select hash transaction value from below output and search same in etherscan to see token distribution. 

```
node distribute.js
```
### To Run through Docker images follow below steps: 
* 1.create Docker file in working directory   
