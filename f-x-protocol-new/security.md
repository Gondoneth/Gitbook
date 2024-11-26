# Security

**Stability Pools(Earn Pools)**

The Stability Pool is a core component of the f(x) protocol, designed to manage risk and reward for each stable-leverage pair while providing participants with opportunities to earn real yields.  By providing a mechanism for rebalancing during times of stress, it ensures the long-term sustainability of stable-leverage pairs. Simultaneously, it rewards participants for their role in maintaining the protocol’s ecosystem.\
\
**Purpose and Functionality**

For every stable-leverage pair in the f(x) protocol, there is a dedicated Stability Pool. This pool serves two primary purposes:

1. To reward stablecoin holders with yields.
2. To act as a buffer against instability when the protocol faces an imbalance.

Stablecoin holders who deposit into the Stability Pool earn rewards generated from the reserve’s staking yields and additional FXN token emissions, offering competitive returns. By doing so, users not only benefit from the protocol’s activity but also contribute to its overall stability.

**Protocol Stability Mechanism**

The Stability Pool becomes critical during periods of potential instability. Instability arises when there is an excessive amount of stablecoins minted compared to the corresponding x-tokens, threatening the balance of the stable-leverage pair. If this situation occurs, the Stability Pool comes into action:

* Stablecoins deposited in the pool are redeemed for reserve assets at their Net Asset Value (NAV).

This redemption process restores balance to the system by decreasing the surplus of stablecoins and reinforcing the reserve assets.

For users, this mechanism operates automatically and effortlessly. It works like buying reserve assets at their exact market value, without any slippage. This guarantees users receive fair value for their stablecoins while helping to stabilize the protocol.

**Yield Farming with Stablecoins**

In normal conditions, when the stable-leverage pair is well-balanced, the Stability Pool operates as a yield-generating vault for stablecoins. Users can deposit their stablecoins to "farm" yields. These rewards are derived from:

1. Staking yields earned by the reserve (stETH).
2. FXN token emissions, which incentivize participation and enhance returns.

This dual-reward structure makes the Stability Pool an attractive option for stablecoin holders seeking higher returns compared to traditional DeFi yield sources.

**Stability Mode**

Stability Mode activates when the system’s reserves, represented by fETH, are worth less than 130% of the stablecoins in circulation (fETH/xETH ratio drops below 1.3) and the Stability Pool runs out of fETH to fix the imbalance.

To handle this, the protocol uses two automated mechanisms funded by treasury revenue. These mechanisms, controlled by on-chain rules, encourage user actions to restore the Collateral Ratio.

**Stabilization Mechanisms**

* xETH Minting Incentives\
  To encourage users to mint more xETH, the protocol temporarily provides a minting bonus, funded by treasury revenue.
* Purpose: Increase the supply of xETH to restore the balance between minted stablecoins and xETH backing.
* fETH Redeeming Incentives\
  To reduce the excess stablecoins in circulation, the protocol offers a redemption bonus for converting fETH back into reserve assets. This bonus is also funded by treasury revenue.
* Purpose: Reduce stablecoin supply and increase reserve assets to improve the CR.

Stability Mode ensures that even in extreme scenarios, the protocol remains robust and self-correcting. These mechanisms act as a final line of defense, maintaining system integrity and protecting users' assets.

**What if bad things happen?**

1. What happens if there’s a huge flash crash in ETH price?

In the unlikely (<0.1%; see whitepaper) event of a price crash in ETH that’s so big that the Stability Pool and minting incentives fail to restabilize the system, the price of xETH can fall to zero \[this is the closest thing to a liquidation on f(x)] and in that case fETH will have sole claim on the reserve. If that happens, the fETH NAV will start following the full price swings of ETH, rather than just 10%. As always, it would be redeemable.

If this ever were to happen there are provisions for recapitalizing the protocol described in the whitepaper.

2. What happens if stETH depegs from ETH?

f(x) has an automatic emergency brake built-in which protects fETH and xETH holders if there is a stETH depeg. Using multiple oracle feeds f(x) can determine if the price of stETH has diverged more than 1% from the price of ETH, and if so minting is (temporarily) disabled. Redemptions remain enabled (as always), however fETH redemptions use the higher of the two prices (stETH, ETH) and xETH redemptions use the lower. When the stETH pegnormalizes, minting resumes. This mechanism ensures fETH and xETH holders are protected, and ensures that no urgent action is ever needed in the event of a stETH depeg.

[Audits](https://github.com/AladdinDAO/aladdin-v3-contracts/tree/main/audit-reports)



\
\


\
\
