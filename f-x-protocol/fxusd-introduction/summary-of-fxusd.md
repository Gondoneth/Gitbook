# Summary of FxUSD

Below is a quick summary of FxUSD, which would help you to understand it easily:

1. Support multiple LSD assets mint and redeem fxUSD
2. Supports Rebalance Pool Earn LSD revenues and FXN mining.
3. fx protocol supports Factory mode which is based on BaseToken, the user can mint corresponding fToken and xToken based on BaseToken deposited.
4. BaseToken's first LSD-enabled assets are frxETH, stETH.
5. Supports BaseToken's LSD gain strategy to get the LSD gain of the underlying asset.
6. fToken is ffrxETH, fstETH respectively. beta=0, initial NAV=$1
7. Users can’t mint fToken directly, users can only mint fxUSD.
8. xToken is xfrxETH, xstETH respectively, initial NAV=$1
9. The rebalance pools supporting fToken are the same with fETH’s Rebalance pools.
10. The FXN emissions of fToken's Rebalance Pool are allocated via gauge weight, with the weight determined by veFXN voting.
11. BaseToken’s Fee is consistent with the existing fETH and xETH fees. Each basetoken corresponds to a fee reserve, which is deposited proportionally to the basetoken. All revenue entering the veFXN Locker Distributor are converted to wstETH.
12. Deposit function supports both zap in and zap out. Supported assets include crvUSD, Frax, USDC, USDT, ETH, frxETH, stETH, ETH.
13. Supports fxUSD (via fToken) swap with xToken.
14. BaseToken needs to satisfy the conditions of the security offer, the Oracle source and the checksum mechanism are as follows.
