# Ethernaut

<p>Ethernaut is a Web3/Solidity based wargame inspired in <a href="https://overthewire.org" target="_blank" rel="noopener noreferrer">overthewire.org</a>, to be played in the Ethereum Virtual Machine. Each level is a smart contract that needs to be 'hacked'.</p>

The game acts both as a tool for those interested in learning ethereum, and as a way to catalogue historical hacks in levels. Levels can be infinite and the game does not require to be played in any particular order.

*Level PR's are welcome!*
Original OZ repository: https://github.com/OpenZeppelin/ethernaut

### Deployed Versions

You can find the current, official version at:
[ethernaut.openzeppelin.com](https://ethernaut.openzeppelin.com)

### Install and build

There are three components to Ethernaut that are needed to run/deploy in order to work with it locally:

·Test Network - A testnet that is running locally, like ganache, hardhat network, geth, etc

·Contract Deployment - In order to work with the contracts, they must be deployed to the locally running testnet

·The Client/Frontend - This is a React app that runs locally and can be accessed on localhost:3000

In order to install, build, and run Ethernaut locally, follow these instructions:

### Running locally (local network)

1. Install
```
git clone https://github.com/esnchez/ethernaut-local-setup.git
yarn install
```
2. Start deterministic rpc
```
yarn network
```
3. You might want to import one of the private keys from ganache-cli to your Metamask wallet.
4. Open a new terminal and let local network running on background. 
5. Compile contracts (to local network) in the new terminal. 
```
yarn compile:contracts
```
6. Deploy contracts
```
yarn deploy:contracts
```
7. Start Ethernaut locally (localhost:3000)
```
yarn start:ethernaut
```
8. Once in client/frontend, select localhost 8545 network in your Metamask wallet. 
9. Deploy challenge contract using the account created in step 3 (get a new instance).
10. Go to ethernaut-solutions repo to run solution scripts. 
