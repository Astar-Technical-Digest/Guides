# Using Hardhat to Deploy To Astar Network

## Introduction

[Hardhat](https://hardhat.org/) is an Ethereum development tools that helps developers manage and be more time efficient while developing their DApps. Hardhat can directly interact with:
- Astar Network
- Shiden Network
- Shibuya testnet

So it can be used to deploy smart into those networks. Astar ecosystem uses [Blockscout](https://blockscout.com/astar/) block explorer and the guide will show you how to automate the recurring tasks to deliver whole solutions much more faster. 

## Prerequisites

To get started, you will need the following:

- Have MetaMask installed and connected to specific network. Let's start with Astar Network mainnet:

`Network`: Astar

`RPC`: https://evm.astar.network

`Chain ID`: 592

`Symbol`: ASTR

Hint: On [Astar Technical Digest](https://twitter.com/AstarTechDigest) Twitter account, you can check up to date MetaMask RPC settings.

## Creation of Hardhat Project

You will need to create a Hardhat project, creation is quite simple, you can do it in the following way:

1. Firstly, you need to create a directory for your project.

`mkdir hardhat-astar-example-project && cd hardhat-astar-example-project`

2. Initialize the projectwhich will create a `package.json` file

`npm init -y`

3. Install Hardhat
   
`npm install hardhat`

I recommend to use `NodeJS` in the version higher or equal to `16.0` and install Hardhat also locally to each project.

Below, you can find settings for networks (click to expand):

<details><summary>Shibuya Settings</summary>
<p>
   
   ```
   Network Name:  Shibuya
   RPC: https://evm.shibuya.astar.network
   Chain ID: 81
   Currency Symbol: SBY
   Block explorer: https://blockscout.com/shibuya/
   ```

</p>
</details>

<details><summary>Shiden Settings</summary>
<p>
   
   ```
   Network Name:  Shiden
   RPC: https://evm.shiden.astar.network
   Chain ID: 336
   Currency Symbol: SDN
   Block explorer: https://blockscout.com/shiden
   ```

</p>
</details>

<details><summary>Astar Settings</summary>
<p>
   
   ```
   Network Name:  Astar Network
   RPC: https://evm.astar.network
   Chain ID: 592
   Currency Symbol: ASTR
   Block explorer: https://blockscout.com/astar
   ```

</p>
</details>

```
shibuya: {
    url: 'https://rpc.shibuya.astar.network:8545',
    chainId: 81,
    accounts: [privateKey]
  },
```

```
shiden: {
    url: 'https://rpc.shiden.astar.network:8545',
    chainId: 336,
    accounts: [privateKey]
  },
```

```
astar: {
    url: 'https://rpc.astar.network:8545',
    chainId: 592,
    accounts: [privateKey]
  },
```

## Verification of a smart contract

https://astar.subscan.io/account/0x101B453a02f961b4E3f0526eCd4c533c3A80d795?tab=contract

## Links

https://docs.astar.network/integration/network-details

https://twitter.com/AstarTechDigest

