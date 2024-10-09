# Farming

Farms are liquidity receipts for LP providers. There exists a farm for each token added to the Omnipool as liquidity. The farm has 2 components:

* Mints 1:1 liquidity receipt ERC-20 tokens for the base token of the farm to LPs. These are called LP tokens. For eg. BTC-LP, ETH-LP, AVAX-LP, DAI-LP etc.
* Accrues fees from actions in the Omnipool which can be redeemed pro-rata by LPs.

LP tokens can be added to the Omnipool and traded themselves, they work just like any other ERC-20 tokens. However, farms do not exist for them as this would introduce an infinite loop of LP positions. Due to their nature, LP tokens introduce their own arbitrage opportunity when their price moves above or below the underlying asset which acts a side profit driver.

The act of depositing in a farm is the same as providing liquidity. The tokens enter the Omnipool and starts earning yield from trading fees.

## Where the yield comes from

* Fee accrual from token swaps
* 50% of borrower interest
* 50%

