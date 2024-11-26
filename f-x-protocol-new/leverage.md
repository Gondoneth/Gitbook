---
description: Where is the Leverage Came From?
---

# Leverage

#### Key Features of fTokens(fETH, fxUSD, btcUSD, ..., etc) and xTokens(xETH, xeETH, xwBTC, ..., etc ):

* fTokens:
  * Fully decentralized and Ethereum, Bitcoin, Convex-native.
  * Minimizes volatility but maintains slight market exposure. (0 volatility except fETH)
  * Instant creation and trading, responding to stablecoin needs.
* xTokens:
  * A perpetual long ETH, BTC, and CVX token with built-in leverage.
  * Composable and fully on-chain with high liquidity.
  * Low liquidation risk, offering a safer alternative for leveraged positions.

**How It Works:**

To mint fTokens or xTokens, users deposit **BaseTokens** (wBTC for btcUSD and xwBTC) into the protocol. This collateral's price volatility is split into, this division allows users to diversify their Basetokens exposure by balancing between stability and leverage, creating a more flexible investment strategy:

* 0% allocated to fTokens (10% for fETH), which absorbs no market volatility.
* 100% allocated to xTokens (90% for xETH), amplifying leverage while maintaining balance.

Fees apply during minting and redemption (0-0.25% for fTokens, 1.5-2.5% for xTokens), but these can be avoided by trading tokens on secondary markets.

