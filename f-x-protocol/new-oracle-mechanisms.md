# New Oracle Mechanisms

Here is a breakdown of the key features and mechanisms of the new oracle solution.

**Enhanced collateral price feeds:** In addition to the original TWAP, spot prices are incorporated, with additional price feeds from Curve, Uniswap V3, and Balancer.

**Arbitrage prevention:** Minting and redeeming transactions are conducted at different prices to eliminate arbitrage trades. This helps to protect the collateral held by the protocol.&#x20;



fToken mint at the minimum price

fToken redeem at the maximum price

xToken mint at the maximum price

xToken redeem at the minimum price



**Risk management:** Collateralized ratio is calculated at maximum price as well as stability pool liquidations. This ensures that risk is managed effectively, and liquidations occur at appropriate levels to maintain system stability.

**Net Asset Value:** NAV is calculated based on TWAP during non-transacting period. This NAV calculation can serve as an oracle price feed for various DeFi applications integrating f(x) assets.

**Additional protection measures for xTokens:** To prevent arbitrage trades, xTokens cannot be both minted and redeemed within the same block. Additionally, a transfer of xTokens cannot occur within a specified timeframe of thirty minutes after minting. These measures help in mitigating potential exploits and maintaining price integrity.



Example:&#x20;

stETH original oracle:&#x20;

1. [stETH/ETH Curve EMA](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit) \* [ETH/USD Chainlink TWAP](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)

stETH new oracle:&#x20;

1. [stETH/ETH Curve EMA](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit) \* [ETH/USD Chainlink TWAP](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)
2. &#x20;[stETH/ETH Curve Spot](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit) \* **ETH/USD UniV3 Spot**&#x20;
3. [stETH/ETH Univ3 Spot](https://info.uniswap.org/#/pools/0x109830a1aaad605bbf02a9dfa7b0b92ec2fb7daa) \* **ETH/USD UniV3 Spot**&#x20;
4. [stETH/ETH Balancer Spot](https://app.balancer.fi/#/ethereum/pool/0x93d199263632a4ef4bb438f1feb99e57b4b5f0bd0000000000000000000005c2) \* **ETH/USD UniV3 Spot**&#x20;
5. [stETH/ETH Curve2 Spot ](https://curve.fi/#/ethereum/pools/steth/deposit)\* **ETH/USD UniV3 Spot**&#x20;

**ETH/USD UniV3 Spot** have 4 price sources, which are:&#x20;

1. [ ](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)[https://data.chain.link/feeds/ethereum/mainnet/eth-usd](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)
2. [https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640](https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640)
3. [https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8](https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8)
4. [https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc](https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc)

Code: [https://github.com/AladdinDAO/aladdin-v3-contracts/pull/198](https://github.com/AladdinDAO/aladdin-v3-contracts/pull/198)

\
\
