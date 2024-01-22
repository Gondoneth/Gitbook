# veFXN Boost Power Shareable Rebalance Pool

**What is that?**&#x20;

The allocation of FXN emissions to individual rebalance pools during each epoch is determined by the corresponding veFXN gauge weight.&#x20;

Rebalance pool is not strictly a gauge as it is not tokenized. Instead, FXN is released by the gauge linearly over a period of 7 days. Subsequently, FXN in the gauge needs to be harvested to the rebalance pool. Upon each harvest, FXN is vested linearly to rebalance pool farmers over 7 days.

The total FXN emissions are proportionally divided based on the farmer's share within the rebalance pool.

However how many FXN tokens each farmer can claim is also determined by his/her veboost power for the epoch. The number of FXN tokens each farmer can claim can vary by 2.5x from the number of FXN tokens earned.&#x20;



**Here is the formula how boost is calculated:**

Boost level = min (Individual TVL x 0.4 + (Total TVL x Individual veFXN for the epoch) x 0.6 / Total veFXN for the epoch, Individual TVL) / (Individual TVL x 0.4)

Claimable FXN = (0.4 x Earned FXN) x Boost Level



**Here Is Some Examples and Corresponding Explanation:**

If a group of farmers share boost power from a veFXN address, the collective TVL is used to calculate the boost level, which is applied to all farmers in the group.

Assume we only have Alice and Bob in the rebalance pool:&#x20;

Example 1

<table data-header-hidden><thead><tr><th></th><th width="165.66666666666666"></th><th></th></tr></thead><tbody><tr><td>Rebalance Pool Farmer</td><td>Alice</td><td>Bob</td></tr><tr><td>TVL $</td><td>100</td><td>100</td></tr><tr><td>Earned FXN for the epoch</td><td>5</td><td>5</td></tr><tr><td>veFXN</td><td>0</td><td>0</td></tr><tr><td>Claimable FXN</td><td>5 x 0.4 = 2</td><td>5 x 0.4 = 2</td></tr></tbody></table>

Example 2

<table data-header-hidden><thead><tr><th width="255"></th><th width="197.66666666666666"></th><th></th></tr></thead><tbody><tr><td>Rebalance Pool Farmer</td><td>Alice</td><td>Bob</td></tr><tr><td>TVL $</td><td>100</td><td>100</td></tr><tr><td>Earned FXN for the epoch</td><td>5</td><td>5</td></tr><tr><td>veFXN</td><td>100</td><td>100</td></tr><tr><td>Claimable FXN</td><td>5</td><td>5</td></tr></tbody></table>

P.S. Total earned FXN for rebalance pool for the epoch is 10 and total veFXN for the epoch is 200.

Curve veCRV is a zero-sum game; people without ve boost power will lose rewards to people who have ve boost power for each epoch. At f(x) rebalance pool, people can lock FXN to earn the maximum rewards they can, and they can do this later on as unclaimed FXN will be reserved till the farmer makes the next transaction, including deposit/withdraw/claim/veFXN boost power top up including receiving shared boost power from another address. \


The system will calculate veFXN for each epoch during the period between two operations (deposit/withdraw/claim/veFXN boost power top-up including receiving shared boost power) and historical boost levels to derive FXN claimable from each historical epoch.



**Here are two examples on how veFXN for historical epochs is calculated:**

Alice locks 100 veFXN in week 1 and another 1000 veFXN in week 4

<table data-header-hidden><thead><tr><th width="142"></th><th></th><th></th><th></th><th></th></tr></thead><tbody><tr><td><br></td><td>Alice’s veFXN</td><td>Total veFXN</td><td>Alice’s retroactive veFXN </td><td>Total retroactive veFXN </td></tr><tr><td>Week 1</td><td>100</td><td>1000</td><td>100</td><td>1000</td></tr><tr><td>Week 2</td><td>99</td><td>990</td><td>99</td><td>990</td></tr><tr><td>Week 3</td><td>98</td><td>980</td><td>98</td><td>980</td></tr><tr><td>Week 4</td><td>97+1000</td><td>970+1000</td><td>1097</td><td>1970</td></tr></tbody></table>

Alice locks 100 veFXN in week 1 and receive veFXN boost power shared in week 4

<table data-header-hidden><thead><tr><th width="117"></th><th></th><th></th><th></th><th></th></tr></thead><tbody><tr><td><br></td><td>Alice’s veFXN</td><td>Total veFXN</td><td>Alice’s retroactive veFXN </td><td>Total retroactive veFXN </td></tr><tr><td>Week 1</td><td>100</td><td>1000</td><td>100</td><td>1000</td></tr><tr><td>Week 2</td><td>99</td><td>990</td><td>99</td><td>990</td></tr><tr><td>Week 3</td><td>98</td><td>980</td><td>98</td><td>980</td></tr><tr><td>Week 4</td><td>97</td><td>970</td><td>97</td><td>970</td></tr></tbody></table>



Boost power shared from another veFXN address will only be applied in the new rewards settlement cycle.

Upon any deposit/withdraw/claim/veFXN top-up transaction including receiving shared boost power, the system will calculate claimable FXN rewards for the period between the two transactions. The difference between earned FXN and claimable FXN, if any, will be transferred to a reserve pool, which will be rolled into the rebalance pool with the condition that the injected additional FXN will not pump the base APR by over 10% for the next epoch.

\
PS: veFXN delegation is not allowed for rebalance pool to prevent arbitrage of rewards

[\
](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_f\(x\)\_Shareable\_RebalancePool\_Report\_20240118.pdf)\
