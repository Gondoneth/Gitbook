# What if bad things happen?

1. What happens if there’s a huge flash crash in ETH price? &#x20;

In the unlikely (<0.1%; see whitepaper) event of a price crash in ETH that’s so big that the Stability Pool and minting incentives fail to restabilize the system, the price of xETH can fall to zero \[this is the closest thing to a liquidation on f(x)] and in that case fETH will have sole claim on the reserve. If that happens, the fETH NAV will start following the full price swings of ETH, rather than just 10%.  As always, it would be redeemable.

If this ever were to happen there are provisions for recapitalizing the protocol described in the whitepaper.\
\


2. What happens if stETH depegs from ETH?

f(x) has an automatic emergency brake built-in which protects fETH and xETH holders if there is a stETH depeg.  Using multiple oracle feeds f(x) can determine if the price of stETH has diverged more than 1% from the price of ETH, and if so minting is (temporarily) disabled.  Redemptions remain enabled (as always), however fETH redemptions use the higher of the two prices (stETH, ETH) and xETH redemptions use the lower.  When the stETH pegnormalizes, minting resumes.  This mechanism ensures fETH and xETH holders are protected, and ensures that no urgent action is ever needed in the event of a stETH depeg.

\
\
