# The Omnipool

## Introducing a new type of AMM infrastructure

The Omnipool is a singleton contract that routes and settles all swaps of tokens (ERC-20 standard). The underlying mechanics are inspired by a mesh of protocol designs from Uniswap and LFJ.

Firstly, liquidity is single sided. Liquidity providers (LPs) can deposit collateral in the form of any ERC-20 token on its own with no need for a two-sided pool by depositing into the relative farm. All token totals are shared within the Omnipool. This key difference compared to traditional AMMs allows for a far greater unlock of liquidity because swaps are no longer only restricted by the capital stored in their respective pools.

To understand how it works, let's first define what a 'swap' is:



## Order types

At the contract level, every swap in the Omnipool is executed as a spot trade for simplicity. However, extra functionality can be added peripherally on top to enable different order types. These are the following order types that are included on the offial BanditDAO UI:

* Spot
* Limit
* DCA
* Perpetual futures
* Options
* Supports trading with up to infinite leverage (upper bounded by the lending supply)



### Global compounding rebase

This is a continuous trigger that can be called by anyone which will rebase the entire protocol. There is an eventual monetary incentive to do so since it internally accrues yield. Thus, it makes sense to call it when the reward outweighs the gas cost.
