# Introduction

## Overview

BanditDAO is a permissionless, non-custodial exchange and yield farming protocol. The core value add is a new type of AMM that introduces single side liquidity, zero impermanent loss, options trading, and zero dependency  on oracles. All features are listed below and explained in detail in their relevant sections:

## Features

* Buy, sell and swap ERC-20 tokens permissionlessly (spot, limit, DCA, leverage, perpetuals)
* Earn fees by providing liquidity with zero impermanent loss.
* Participate in farms to earn rewards.
* Trade call and put options on any asset.
* Earn interest on your favorite tokens (BTC, ETH, DAI etc.).
* Borrow assets (DAI, BTC, AVAX etc.) with no liquidations.
* Stake BNDT to earn relative payouts in DAI, BTC, AVAX and more.

## An actual DAO

This project is 100% decentralized and open source. We are what an actual 'DAO' should be: There is no multisig, dev ownership or team allocation. Nothing like that. The contracts and changeable mechanisms are in the hands of the community. Read more on how we handle governance->

## Contracts

The protocol is designed to be lightweight and simple to understand for even a layperson to be able to read the contracts.

#### Core:

* Omnipool.sol: Handles all trading infrastructure including farms
* Loaner.sol: Handles lending and borrowing
* Treasury.sol: Handles staking, token minting and protocol rewards

**Tokens:**

* BNDT.sol: Native base token
* stBNDT.sol: The staked receipt of BNDT
* wstBNDT.sol: A wrapper for sBNDT that accrues yield internally so it can be used externally (for eg. deposited in a farm)

### Note for developers wanting to build and contribute

We highly encourage users to build infrastructure on top of BanditDAO's core functionality, on top of the Omnipool for example. To introduce cool projects and added functionality on top of these base designs is exactly what we want to happen. We happily encourage forks of the project to add your own use cases and extend features to expand the user base and build your own.

