# fToken Rebalance Pool

The fToken Rebalance Pool consists of two components: the ffrxETH Rebalance Pool and the fstETH Rebalance Pool.

Here is how Rebalance Pool Deposit & Earn works, it is built to support for earning rewards by minting fToken with BaseToken and depositing it into. Users may:

1. Mint fToken with BaseToken and deposit it into the rebalance pool.
2. Zapping in BaseToken, such as crvUSD, Frax, USDC, USDT, ETH, frxETH, stETH, or ETH, and simultaneously minting fToken and depositing it into the rebalance pool.
3. Directly depositing fxUSD into the rebalance pool using the corresponding fToken. If there is insufficient fToken under fxUSD, only the corresponding maximum amount of fToken can be deposited into the rebalance pool.

Deposit & Earn Process: fxUSD -> fToken -> BaseToken -> Rebalance Pool, Users cannot deposit into the corresponding rebalance pool if fToken is below $1.

#### Rebalance Pool Withdrawal of fxUSD&#x20;

Protocol supports three types of rebalance pool withdrawals:

1. fxUSD: Withdraw fToken from the rebalance pool and mint fxUSD.
2. BaseToken: Withdraw fToken from the rebalance pool and redeem fToken to obtain the corresponding BaseToken.
3. USDC, USDT, ETH: Withdraw fToken from the rebalance pool and redeem fToken to obtain the corresponding BaseToken. Zap out into crvUSD, Frax, USDC, USDT, ETH, frxETH, stETH, or ETH.

#### Rebalance Pool Share&#x20;

Protocol supports the sharing of veFXN functionality. Owners can share their veFXN with other users (stakers). Stakers receiving the owner's veFXN have their boost ratio calculated based on the owner's boost ratio, which includes the staker's fToken balance. Ve sharing supports whitelist functionality, where only whitelisted owners can share veFXN voting power.

The above functionalities also apply to fETH's rebalance pool.
