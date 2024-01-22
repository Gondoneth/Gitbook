# f(x) Protocol

## Abstract

f(x) Protocol creates two new ETH derivative assets, one with stablecoin-like low volatility and the second a leveraged long ETH perpetual token. These tokens are created by separating ETH collateral into a lower-volatility component (β < 1) called fractional ETH (fETH) and a higher-volatility (β > 1) one called leveraged ETH (xETH). By constraining βf = 0.1 the fractional ETH token captures some growth of the cryptocurrency market while limiting volatility enough to retain the characteristics of a stablecoin. The leveraged ETH component is essentially a long perpetual future contract with zero funding costs and variable leverage. The system is backed exclusively by a mixture of pure ETH and selected highly liquid staked ETH derivative collateral tokens, which means it is not exposed to centralized risk from real-world assets. Maximum liquidity of fETH can scale quickly compared with CDP-issued stablecoins because it is based on the high demand for leveraged long ETH positions (xETH) rather than the relatively lower demand for CDPs, with their attendant maintenance and capital inefficiency.

## Introduction

&#x20;Stablecoins are an essential enabling technology for decentralized finance (DeFi). They enable fully on-chain swaps in and out of fiat denomination as well as the creation of a wide array of powerful decentralized financial instruments. Additionally, due to the volatility of all cryptocurrencies, even the most crypto-native of organizations and individuals must plan for expenses in fiat terms, and must therefore hold at least some fiat-denominated reserve. Despite the critical importance of these tokens, they have also introduced new risks and been responsible for some of the DeFi’s most damaging failures. Pure algorithmic stablecoins have failed so spectacularly that little needs to be said about their risk, but current stablecoin implementations suffer from critical weaknesses which will ultimately hinder their long-term success. The majority of use cases for stablecoins do not require a hard peg to a specific fiat currency so much as they require low volatility against fiat generally. In this document we will introduce a protocol that uses a unique mechanism to create two new ETH derivative tokens: fETH, a low β near-stablecoin, and xETH, a high β leveraged long ETH perpetual contract. The leveraged long token offers a powerful new decentralized tool for on-chain trading while the low volatility token provides an alternative to current stablecoin offerings that eliminates centralized risk while also being able to scale efficiently enough to meet the needs of the DeFi industry.&#x20;

## Stablecoin Risks and Scaling&#x20;

The most obvious type of risk seen in recent years in stablecoins is in pure algorithmic (underor un-collateralized) implementations, of which UST by Terra is the most obvious example. Making this type of stablecoin safe and reliable may very well be impossible, but for the purposes of this discussion we consider this class of stablecoin so risky as to immediately disqualify it from being a good choice for long-term reliability. 1 Among remaining designs, there are currently three broad categories of stablecoins in the market:

1. Fiat-backed stablecoins (USDC, USDT)
2. Algorithmic, but fully or partly collateralized by fiat-backed stablecoins (DAI, FRAX)
3. Fully decentralized CDP algorithmic stablecoins (LUSD) Categories (1) and (2) both suffer from centralization risk, while category (3) has, as yet, struggled with scalability and capital efficiency compared to those in (1) and (2). These centralization risk and scaling challenges leave the door open for other solutions.

{% embed url="https://fx.aladdin.club/home/" %}
