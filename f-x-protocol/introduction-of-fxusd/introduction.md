# Introduction

Hence, the innovative, dynamic stable-leverage pair technology provides three crucial features to fxUSD:

1. Powerful, real-world-proven peg that protects from both upwards and downwards depegs
2. Built-in real yield, denominated in the reserve’s yield (staked ETH, in this case)
3. Instant mint-and-redeemability with zero slippage and no swap pool liquidity required (especially once integrated to aggregators, note fees still apply)

An important difference from fETH/xETH to fxUSD, and indeed for all new stable-leverage pairs except for fETH going forward, is that the stable derivative tokens of a single reserve will not be liquid. Instead, they can only exist in the Stability Pool or (if the pair is included in fxUSD backing) in the fxUSD reserve. Stability Pool stable deposits can be redeemed for their share of the reserve at any time without limit, but not withdrawn to a wallet on their own. Stables from pairs which back fxUSD can be withdrawn from the Stability Pool, or even minted directly… but only as fxUSD.

Using only the mechanism described above, every stable-leverage pair creates two derivative tokens plus its own Stability Pool. For the purposes of scaling, however, f(x) should have only one USD-pegged stablecoin. To achieve this, individual reserve stablecoins will not be liquid, but instead will be limited to either farming in its Stability Pool or being used to mint the single liquid king-token: fxUSD. Stability Pools and leveraged tokens will still be separate for each reserve LSD, allowing varying yields between stability pools, as well as varying leverage between each leveraged “x” token. This separation is sensible since those pools and tokens are backed by different reserve LSDs with different risks, base yields, etc.

fxUSD consolidates stablecoins from constituent pairs as follows:

1. fxUSD is backed 1:1 by a basket of stables from accepted LSD stable/leverage pairs, and can be minted by supplying an accepted LSD or by withdrawing from a rebalance pool
2. When minting fxUSD from an LSD, the LSD is used to mint the stable derivative of that LSD, which is then placed in the fxUSD reserve
3. When minting fxUSD by withdrawing stables from a rebalance pool, the withdrawn stables are moved to the fxUSD reserve

\
\
