# BNDT

BNDT is a deflationary ERC-20 token with an internal growth mechanism (see more ->). BNDT is minted at a 1:1 ratio to deposits of DAI, FRAX and USDC to the Treasury. This forms the backing of BNDT wherein the treasury will hold these stablecoins of equal supply to the supply of BNDT. Therefore, if the price of BNDT somehow drops below 1 DAI, 1 FRAX or 1 USDC (for simplicity we will say $1 USD from here on) it can be burned to the Treasury for a profit. This is the monetary incentive that forms the price floor of $1. DAI, FRAX and USDC were chosen as they are reliable stablecoins trusted by the crypto community in large.

However, this 1:1 ratio can increase. It can increase at a rate chosen by the community at their discretion through governance. However it cannot go below $1. 1:1 is the ratio it is set to at genesis ie. when the contracts are first deployed.

The supply of BNDT is designed to expand with the expansion of treasury profit. The DAI, FRAX, and USDC balance of the treasury thus can increase above the minting ratio. If the price of BNDT goes above this ratio, the treasury mints BNDT until the supply ratio is equal again. 100% of this minted BNDT is queued for release to stakers. This also has an intended side consequence where the price of BNDT should theoretically then decrease back down to a more sustainable level closer to the minting ratio.



The main incentive to buy BNDT is it can be staked to receive more BNDT when minting expansions occur but mainly to earn a profit share of the treasury's LP ownings.
