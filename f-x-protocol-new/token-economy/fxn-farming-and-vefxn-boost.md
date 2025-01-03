# FXN Farming and veFXN Boost

The [FXN overall token allocation](https://medium.com/@protocol_fx_667/f-x-protocols-tokenomics-offer-a-calculated-journey-towards-success-b97487df41b9) specifies 980,000 FXN tokens (49% of max supply) to be emitted as liquidity incentives over a 50-year period, with the emission rate starting at 98,000 FXN for the first year and declining by 10% (relative) each year thereafter. Each year is divided into weekly epochs, with a veFXN governance vote determining how that epoch’s FXN will be allocated among the available gauges, the same as in the Curve’s pioneering model. In the details, however, there are several differences to Curve, driven by technical considerations in the f(x) system.

**Gauge Types**

f(x) Protocol supports two types of gauges: Stability Pool gauges, and liquidity pool gauges. For LP gauges, farmers can earn FXN by providing liquidity to certain Curve liquidity pools. These gauges are based on a double-gauge structure: farmers stake their Convex farming positions, allowing them to earn **both** Curve/Convex rewards as well as FXN. Of course, zaps hide this complexity for users who wish to simply deposit underlying tokens. LP gauge yields are boosted by owned, shared or delegated veFXN boost.

On the other side, Stability Pools are even more different to Curve gauges. First, they are not strictly gauges in the Curve sense, due to the fact that they are not tokenized. This has implications for how tokens are distributed, how boost is allocated, and more. Additionally, Stability Pool gauges can be boosted by owned or shared veFXN boost, but not delegated.

**Boost Calculation**

In Curve’s gauge model, all gauge emissions are distributed immediately and users with boost power take rewards from users without. The veFXN model allows each user to earn their own maximum FXN, and if they do not, the difference is rolled over and used to increase yields for the pool across the board.

FXN distributions to the Stability Pool are shared among farmers according to each farmer’s share of TVL in that pool and their share of total veboost power. Each farmer’s share of TVL in the pool determines the maximum share of incoming FXN they can earn, while their boost determines how much of that they can actually claim. Farmers with veboost power earn up to 2.5X more than farmers with none.

Farmers who have zero veboost have a boost of 1X, which allows them to claim 40% of their maximum earnable share of FXN for this epoch. Farmers who have the maximum veboost of 2.5X may claim 100% of their maximum share.

Each farmer’s boost level is calculated like this:

Maximum FXN = Total Distributable FXN x Individual TVL / Total TVL

Claimable FXN = 0.4 x Maximum FXN x Boost Level

Boost Level = min (Individual TVL x 0.4 + (Total TVL x Individual veFXN for the epoch) x 0.6 / Total veFXN for the epoch, Individual TVL) / (Individual TVL x 0.4)

An alternative way to think about boost level is in terms of two variables: A farmer’s fractional share of the total veboost (fv), and a farmer’s fractional share of the total TVL (fd). Using these terms, each farmer’s boost is calculated like this:

![](https://docs.aladdin.club/~gitbook/image?url=https%3A%2F%2Flh7-us.googleusercontent.com%2FzigI0vGIQ3AI-ZKpjgp-3-i_rDOvfqAuKwCIURg-HqYGXKRHCqntLQ6sQNkvhaIOyggsaVs5eYwSQmuEMszVn3YeZfnF0IH4rq3Nmf-IfD8J5BPfVu1hNyBkAdb-yOaFyQ8iAR-M8kYeXsRa2f2Hgak\&width=300\&dpr=4\&quality=100\&sign=6f71ad32\&sv=1)

For an individual farmer, the optimal approach is to hold precisely the same share of the total vepower and TVL. A higher share of total vepower than their share of the TVL doesn’t help that farmer, however, the FXN system allows sharing boost power for whitelisted addresses (see below).



**Rollover FXN**

It is likely that not every farmer will earn their maximum share, which means each time a farmer in the pool makes a settlement transaction (see “Settlement”) there may be leftover FXN. This leftover FXN is rolled forward and treated as a new distribution to the Stability Pool, similar to FXN coming from the gauge.

When any new FXN comes to the Stability ool it is combined with FXN already vesting (if any), and the sum is vested over a new 7 day period starting at the moment of the distribution. Since distributions can come from settlement transactions at any time and in any amount, it would be possible for a small distribution to come in at an inopportune time and artificially (briefly) deflate the pool APR.

To prevent this, FXN rollover distributions which would cause the overall pool APR to drop more than 10% are held in reserve, and added to the next settlement-triggered distribution.

**Sharing and Delegating Boost Power**

A whitelisted address can choose to share its veFXN boosting power with one or more other addresses. This mechanism is useful for boosting services built on top of f(x), allowing many individual farmers to benefit from a single central pool veFXN. In the case of shared boosting, the total veboost is calculated using the amount of veFXN shared (i.e. that held by the sharing address) and the collective TVL of the all recipients. The calculated boost level is applied to all recipients.

Users may also choose to delegate their veFXN boost power to another single address. Delegated boost can be used to boost LP farming yields, but not stability pool yields.

**Emissions Require Harvesting**

A Stability Pool is not strictly a gauge in the Curve sense because it is not tokenized. This has some technical implications, but practically it means the following:

1. FXN is released by the gauge linearly over a period of 7 days, but requires harvesting before it can be distributed
2. FXN is minted when the harvest function is called (it is a permissionless keeper function). Minted FXN is vested linearly to Stability Pool farmers over 7 days.

Between harvest delays and vesting, token emissions have smoothed and slightly delayed changes from pool APRs. Things will smooth out after a week.

**Settlement**

Upon any deposit/withdraw/claim/veFXN top up transaction (including receiving shared boost power,) the system will immediately calculate and settle claimable FXN rewards for the period between two transactions. Even though a user may not choose to make any transaction which triggers settlement for a period of many epochs, the amount of FXN they may claim from each past epoch is locked in and does not change after the end of that epoch. In other words, when the settlement happens, total claimable FXN for each epoch since the previous settlement is calculated using TVL and veboost values from that epoch.

Settlement happens prior to the execution of the transaction which triggers it, so any changes to veboost which result from the transaction will apply only to subsequent epochs.

**Examples**

Here are two simple numerical examples. Assume we only have Alice and Bob in the Stability Pool, and that there are 10 distributable FXN for this epoch:

Example 1 (nobody has any veboost)

| Stability Pool Farmer              | Alice       | Bob         |
| ---------------------------------- | ----------- | ----------- |
| TVL $                              | 100         | 100         |
| Maximum Earnable FXN for the epoch | 5           | 5           |
| veFXN                              | 0           | 0           |
| Claimable FXN                      | 5 x 0.4 = 2 | 5 x 0.4 = 2 |

In Example 1, only 4 out of 10 FXN have been distributed, so the remaining 6 FXN are placed in the rollover reserve which will be used to increase distributable FXN in later epochs.

Example 2 (everybody has equal veboost)

| Stability Pool Farmer              | Alice             | Bob               |
| ---------------------------------- | ----------------- | ----------------- |
| TVL $                              | 100               | 100               |
| Maximum Earnable FXN for the epoch | 5                 | 5                 |
| veFXN                              | 100               | 100               |
| Claimable FXN                      | 5 x 0.4 x 2.5 = 5 | 5 x 0.4 x 2.5 = 5 |

All of the 10 FXN have been distributed when everybody has the equal veboost.

