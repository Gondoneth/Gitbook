# fxUSD Reserve and Risk Management

#### The fxUSD Reserve

fxUSD is backed 1:1 by a reserve of $1-pegged stables from whitelisted ETH LSD stable-leverage pairs, beginning at launch with stETH and sfrxETH.  Since the fxUSD reserve is separate from the constituent stable-leverage pairs, stable tokens from whitelisted pairs can exist in its rebalance pool or the fxUSD reserve, but not both.

<figure><img src="https://lh7-us.googleusercontent.com/XevGO1klvlS_jL9ifJrMgLnIb2pyyXDmfmKB5tntgwyrch_MITr1IfwCjMq77V5eaygo55joiWIJm60q5q6NyszpckjbZ9S0UqFwIQFpFTnGbqMSIvZAOqgvvdBfTeSKzrH3i26fU3CaU90yaeAWilk" alt=""><figcaption></figcaption></figure>

Once minted, fxUSD can be held in a wallet, transferred, used outside f(x), etc.  fxUSD can also be deposited back into one of the source rebalance pools or redeemed for reserve ETH LSD tokens.  The availability of rebalance pool and reserve token redemption paths depends on the token makeup of the fxUSD reserve, which can vary. Since fxUSD is minted 1:1 against tokens in its reserve there is always a way to redeem every fxUSD for $1 worth of an ETH LSD, though which specific LSDs are available for redemption depend on which stables are present in the fxUSD reserve.  Likewise, fxUSD can only be directly “deposited” (i.e. redeemed for LSD-stables and moved) to a rebalance pool if there are appropriate tokens available in the fxUSD reserve.

<figure><img src="https://lh7-us.googleusercontent.com/iGOtUfOhCqoHynrNfpoTZB09iyNAvLy7DnrcPcvV1I6lnwL6mGt0p957tFOukg-8EEasbVOwXxO99YuVgdwNnUGqD-p72TQ3vFI6YhrAYu1m-Ojh6FXv7gRZTlnMqQIZuheZvCuS9-C0vLCLQaCp15U" alt=""><figcaption></figcaption></figure>

Consider an example. Starting from an empty fxUSD reserve, imagine Alice mints 100 fxUSD using stETH-Stable, and Bob mints 10 fxUSD using frxETH-Stable.  Alice can then deposit up to 10 fxUSD into the frxETH-Stable pool (and perhaps redeem those for frxETH).  If she does so, then all the remaining fxUSD, including Bob’s 10 fxUSD, can only be deposited into the stETH Rebalance pool, to be redeemable for stETH.

#### Risk Management

fxUSD risk management begins with the already very robust risk management of the f(x) stable-leverage pair (see the [whitepaper](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/whitepapers/f\(x\)\_whitepaper\_v2.pdf)).  Beyond this, the main risk management strategy at the fxUSD level is the careful controlling of which tokens to accept in the reserve.  New LSDs may be onboarded to expand the fxUSD reserve at some point, but each new backing LSD will be subject to risk management review, parameter setting and community governance approvals prior to being allowed into the fxUSD reserve. &#x20;

Additionally, the system can temporarily disable fxUSD minting to keep all depositors safe in the case of a serious problem with a constituent stable-leverage pair.  The two cases where this happens are if the underlying LSD reserve token depegs from ETH, or if the collateralization ratio falls below 100% (which can only happen after rebalance pool redemptions and all other risk mitigations fail).  Since rebalance pools hold stables from the underlying SLP and not fxUSD, disabled minting also disables rebalance pool withdrawals to fxUSD.  Redeeming fxUSD or rebalance pool deposits for reserve tokens is, as always, still possible.

\
\


\
\
