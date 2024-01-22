# The CLever

### <mark style="color:blue;">Why use CLever?</mark>

1. Your future yield “loan” is non liquidating, low risk, has certainty in funding costs, and is automatically paid down as yields are harvested from your collateral.
2. For CVX, yield harvesting is fully automated and gas prices are shared between all users. Locking, voting, collecting bribes, even re-locking in Convex as needed is all automatic.

### <mark style="color:blue;">How does it work?</mark>

Users lock their collateral Token in a yield strategy, then can immediately claim some of their future yields as clevToken for zero cost (except gas). clevTokens can be farmed or swapped for equivalent Tokens using either the Curve liquidity pool or the Furnace. To create leverage, users may re-deposit their Token to earn even more.

Behind the scenes, yields from the collateral strategy are swapped back to the collateral token and used to pay down the user’s debt to the system.

### <mark style="color:blue;">What is clevCVX, clevUSD, etc?</mark>

clevTokens are synthetic versions of their associated real token, representing the future yield of CLever strategies. Each clevToken is backed by one or more equivalent real Tokens in the system. These tokens can be farmed in CLever liquidity pools or swapped for more of the original token.

### <mark style="color:blue;">How are yields harvested?</mark>

Each collateral strategy has its own yield harvesting mechanism. In the case of the CVX strategy, CVX locked with CLever will itself be vote-locked in Convex and used to vote for **maximum bribe income**.

<figure><img src="../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

### <mark style="color:blue;">Can I withdraw my collateral?</mark>

Each collateral strategy has a maximum debt ratio which must be maintained, so you may withdraw only as much collateral as keeps you under the maximum debt ratio. For a fee you can repay your loan early to withdraw your collateral sooner.

For collateral strategies which require an underlying lock, such as CVX -> vlCVX in Convex, users must request an unlock and wait for the underlying unlock before withdrawing. Collateral does not earn yield after unlock has been requested.

### <mark style="color:blue;">Is this a loan?</mark>

Yes, you can think of it that way. Your locked CVX is the collateral, and the yields from it automatically pay down your debt… but CLever loans are special and offer what we think is the best risk/reward profile for borrowing in all DeFi. Our technique of using a synthetic token paired with a real one (i.e. clevCVX with CVX) offers several advantages:

1. No liquidations, ever&#x20;
2. No oracle price feeds needed to monitor loan health&#x20;
3. Borrowers only take risk of their chosen collateral (as opposed to all assets accepted by protocol, like with stablecoin borrowing or CDPs)&#x20;
4. Funding cost is fixed and doesn’t fluctuate with liquidity adding/removal/utilization

### <mark style="color:blue;">Can I repay my claimed future yields early?</mark>

Yes, claimed future yields may be repaid any time directly in clevCVX or CVX (1:1). Note that any early repayment is subject to a fee (see fees below).

### <mark style="color:blue;">Are you trying to trick me into giving you my CVX/other collateral? Or using my CVX to vote for your thing?</mark>

No. Users retain ownership of their locked collateral, and can withdraw if they choose (see Can I Withdraw…). For CVX, votes are cast to maximize bribe value (initially by delegating to Votium).

### <mark style="color:blue;">Is it safe?</mark>

CLever is built by the experienced and security-obsessed AladdinDAO team and is audited by SECBIT Labs. The audit is [here](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_CLever\_Report\_v1.1.pdf). This is the Aladdin way.

### <mark style="color:blue;">How much does it cost?</mark>

CLever charges a fixed fee on collateral yields when they are harvested. This fee will vary by strategy, but for CVX it is 20% of the harvested amount. 75% of harvest fees are paid to veCLEV holders, providing major support to the value of CLEV which is used to incentivize crucial liquidity providers. **CLever charges no fee on principal, no borrowing fee and no interest on borrowed tokens.**

CLever's CVX harvest fee is 20% of yields harvested.

CLever's Frax harvest fee is 10% of yields harvested.

CLever's CVX early repayment of claimed future yields are subject to a 1% repayment fee.

CLever's Frax early repayment of claimed future yields are subject to a 0% repayment fee.

### <mark style="color:blue;">What can i do with my CLEV?</mark>

There are a number of ways you can use CLEV to earn and govern:

Provide liquidity in CLEV-ETH pool on Curve and stake the LP token on CLever to earn liquidity mining rewards, more CLEV!

Vote lock CLEV to earn a boost of up to 2.5x liquidity mining rewards and earn system revenue! CLever will distribute 75% of its revenue to veCLEV holders. This will be turned on very soon.

Vote lock CLEV to acquire voting power and participate in community governance.

