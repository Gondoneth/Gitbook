# The background of FxUSD (Why do we need it?)

f(x) Protocol introduced fETH and xETH as well as the overall concept used to create them: the stable-leverage pair. To understand fxUSD, that is where we begin.

To create a stable-leverage pair, f(x) holds a reserve of some base token. To start, let’s consider stETH. Minted against that stETH reserve are two types of derivative tokens; one stable, and one volatile. At all times, the total market cap of the two derivative tokens is held equal to the value of the reserve, and any derivative token can be redeemed at any time for its share of the reserve base token.

As the price of the reserve token varies, so too does the amount of base token a user may redeem for each of the stable and volatile tokens. The stable token is held fixed at a USD value of $1, so as the price of stETH in the reserve rises, the volatile token price rises at a multiple rate of stETH. Based on the performance of xETH, this multiple generally varies between 1.5x — 4x though though it can rise as high as 4.3X before the protocol responds to limit it.

<figure><img src="https://lh7-us.googleusercontent.com/EhqZnMikxz2_Xv_TsbJ3tXqMhjgAp7VHIC1K9jf5VOTLgtxTV_StAqd9YlhiCY_kMYJa3qrfKQhjlgUopgt94pyLOMFmLn6KLS5tUocKjLZBsUDCy3eZaPthiovF8jfCXyiL8u4Eq9LQwbmjJ5kSIY4" alt=""><figcaption></figcaption></figure>

To maintain the stability of the overall system, a “Stability Pool” is provided. By depositing the stable derivative tokens in the rebalance pool, users can earn a share of the yield from the reserve, i.e. the stETH staking yield. In exchange for this yield the users take a risk: if there is ever too much of the stable token and not enough of the volatile one to absorb volatility, stables from the Stability Pool are redeemed for stETH from the reserve, thus relieving pressure on the volatile token and maintaining the stability of the system. From a user’s perspective, this is equivalent to buying stETH at market price with the stables in the stability pool.

\
\
