# Oracles

## Oracle Mechanisms

Here is a breakdown of the key features and mechanisms of the oracle solution.

**Enhanced collateral price feeds:** In addition to the original TWAP, spot prices are incorporated, with additional price feeds from Curve, Uniswap V3, and Balancer.

**Arbitrage prevention:** Minting and redeeming transactions are conducted at different prices to eliminate arbitrage trades. This helps to protect the collateral held by the protocol.

fToken mint at the minimum price

fToken redeem at the maximum price

xToken mint at the maximum price

xToken redeem at the minimum price

**Risk management:** Collateralized ratio is calculated at maximum price as well as stability pool liquidations. This ensures that risk is managed effectively, and liquidations occur at appropriate levels to maintain system stability.

**Net Asset Value:** NAV is calculated based on TWAP during non-transacting period. This NAV calculation can serve as an oracle price feed for various DeFi applications integrating f(x) assets.

**Additional protection measures for xTokens:** To prevent arbitrage trades, xTokens cannot be both minted and redeemed within the same block. Additionally, a transfer of xTokens cannot occur within a specified timeframe of thirty minutes after minting. These measures help in mitigating potential exploits and maintaining price integrity.

### **\[ETH/USD Spot]** have 4 price sources, which are: <a href="#eth-usd-spot-have-4-price-sources-which-are" id="eth-usd-spot-have-4-price-sources-which-are"></a>

* [https://data.chain.link/feeds/ethereum/mainnet/eth-usd](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)
* [https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640](https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640)
* [https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8](https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8)
* [https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc](https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc)

### stETH oracle: <a href="#steth-new-oracle" id="steth-new-oracle"></a>

1. \[[stETH/ETH Curve EMA](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit) ]\*\[[ETH/USD Chainlink TWAP](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)]
2. \[[stETH/ETH Curve Spot](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit)] \* \[**ETH/USD Spot** ]
3. \[[stETH/ETH Univ3 Spot](https://info.uniswap.org/#/pools/0x109830a1aaad605bbf02a9dfa7b0b92ec2fb7daa)] \*\[ **ETH/USD Spot** ]
4. \[[stETH/ETH Balancer Spot](https://app.balancer.fi/#/ethereum/pool/0x93d199263632a4ef4bb438f1feb99e57b4b5f0bd0000000000000000000005c2)] \* \[**ETH/USD Spot** ]
5. \[[stETH/ETH Curve2 Spot\] ](https://curve.fi/#/ethereum/pools/steth/deposit)\* \[**ETH/USD Spot ]**

### frxETH oracle: <a href="#frxeth-new-oracle" id="frxeth-new-oracle"></a>

1. \[[Curve frxETH/WETH EMA](https://curve.fi/#/ethereum/pools/factory-crvusd-15)] \* \[[Chainlink ETH/USD TWAP](https://etherscan.io/address/0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419)]
2. \[[Curve frxETH/WETH Spot](https://curve.fi/#/ethereum/pools/factory-crvusd-15)] \* \[**ETH/USD Spot** ]
3. \[[Curve frxeth Spot](https://curve.fi/#/ethereum/pools/frxeth)] \* \[**ETH/USD Spot** ]
4. \[[Curve stETH/frxETH Spot](https://curve.fi/#/ethereum/pools/factory-v2-274)] \* \[[Curve steth Spot](https://curve.fi/#/ethereum/pools/steth/deposit)] \* \[**ETH/USD Spot** ]

### weETH oracle: <a href="#weeth-new-oracle" id="weeth-new-oracle"></a>

1. \[[RedStone weETH/ETH Twap](https://etherscan.io/address/0x8751F736E94F6CD167e8C5B97E245680FbD9CC36)] \* \[[Chainlink ETH/USD TWAP](https://etherscan.io/address/0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419)]
2. \[[Uniswap V3 ETH/weETH 0.05%](https://info.uniswap.org/#/pools/0x7a415b19932c0105c82fdb6b720bb01b0cc2cae3)] \* \[**ETH/USD Spot** ]/weETH.getRate()
3. \[[Uniswap V3 wstETH/weETH 0.05%](https://info.uniswap.org/#/pools/0xf47f04a8605be181e525d6391233cba1f7474182)] \*\[wstETH/stETH rate] \* \[ [Curve steth-ng](https://curve.fi/#/ethereum/pools/factory-v2-303)]\* \[**ETH/USD Spot** ]
4. \[[Curve weETH/ETH](https://curve.fi/#/ethereum/pools/factory-stable-ng-22)] \* \[**ETH/USD Spot** ]

### ezETH oracle: <a href="#ezeth-new-oracle" id="ezeth-new-oracle"></a>

1. \[[RedStone ezETH/ETH Twap](https://etherscan.io/address/0xF4a3e183F59D2599ee3DF213ff78b1B3b1923696)] \* \[[Chainlink ETH/USD TWAP](https://etherscan.io/address/0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419)]
2. \[[Curve ezETH/ETH](https://curve.fi/#/ethereum/pools/factory-stable-ng-79/deposit)] \* \[**ETH/USD Spot** ]
3. \[[Balancer V2 Stable](https://app.balancer.fi/#/ethereum/pool/0x596192bb6e41802428ac943d2f1476c1af25cc0e000000000000000000000659)] \* \[**ETH/USD Spot** ]

### WBTC oracle: <a href="#wbtc-new-oracle" id="wbtc-new-oracle"></a>

1. \[[Chainlink WBTC/BTC Twap](https://data.chain.link/feeds/ethereum/mainnet/wbtc-btc)] \* \[[Chainlink BTC/USD Twap](https://data.chain.link/feeds/ethereum/mainnet/btc-usd)]
2. \[WBTC/USDC spot price of [Curve TriCryptoUSDC](https://curve.fi/#/ethereum/pools/factory-tricrypto-0)]
3. \[[Uniswap V3 WBTC/USDC 0.3% Spot](https://info.uniswap.org/#/pools/0x99ac8ca7087fa4a2a1fb6357269965a2014abc35) ]
4. \[[Uniswap V3 WBTC/ETH 0.3% Spot](https://info.uniswap.org/#/pools/0xcbcdf9626bc03e24f779434178a73a0b4bad62ed)] \* \[[Uniswap V3 USDC/ETH 0.05% Spot](https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640)]

### CVX oracle: <a href="#cvx-oracle" id="cvx-oracle"></a>

1. \[[Chainlink CVX/USD Twap](https://data.chain.link/ethereum/mainnet/crypto-usd/cvx-usd)]
2. \[[Chainlink CVX/USD Spot](https://data.chain.link/ethereum/mainnet/crypto-usd/cvx-usd)]
3. \[[Curve CVX/ETH](https://curve.fi/#/ethereum/pools/cvxeth/deposit)] \* \[**ETH/USD Spot** ]

Code: [https://github.com/AladdinDAO/aladdin-v3-contracts/pull/198](https://github.com/AladdinDAO/aladdin-v3-contracts/pull/198)



## **Oracle of F(x) 2.0**

Below is the breakdown of stETH Spot price **Oracle Mechanism**:

### \[ETH/USD Spot] oracle:

* [https://data.chain.link/feeds/ethereum/mainnet/eth-usd](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)
* [https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640](https://info.uniswap.org/#/pools/0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640)
* [https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8](https://info.uniswap.org/#/pools/0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8)
* [https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc](https://v2.info.uniswap.org/pair/0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc)

### \[stETH/ETH Spot] oracle:

* \[[stETH/ETH Curve Spot](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit)]&#x20;
* \[[stETH/ETH Univ3 Spot](https://info.uniswap.org/#/pools/0x109830a1aaad605bbf02a9dfa7b0b92ec2fb7daa)]&#x20;
* \[[stETH/ETH Balancer Spot](https://app.balancer.fi/#/ethereum/pool/0x93d199263632a4ef4bb438f1feb99e57b4b5f0bd0000000000000000000005c2)]&#x20;
* \[[stETH/ETH Curve2 Spot\]](https://curve.fi/#/ethereum/pools/steth/deposit)&#x20;

### \[stETH/USD] Anchor Price oracle(It is a backup price feed):

* \[[stETH/ETH Curve EMA](https://curve.fi/#/ethereum/pools/factory-v2-303/deposit) ]\*\[[ETH/USD Chainlink Spot](https://data.chain.link/feeds/ethereum/mainnet/eth-usd)]

### The Algorithm of stETH/USD Max and Min Price:

* Max stETH/USD Price=Max(Anchor Price, \[stETH/ETH Spot Max Price ]\* \[ETH/USD Spot Max Price ])
* Min stETH/USD Price=Min(Anchor Price, \[stETH/ETH Spot Min Price ]\* \[ETH/USD Spot Min Price ])

### Price Checking Mechanism:

* Anchor Price is used, while the price difference between Anchor Price and Max/Min Price exceeded **threshold**
* **threshold** is an exchangeable parameter in future governance proposals, 2% in default

### Conclusion:

* **Min** stETH/USD **Price** is used while Rebalancing, Minting/Redeeming of xPOSITION, and the price difference between Anchor Price and Min Price **didn't** exceed **threshold**
* **Anchor Price** is used while Rebalancing, Minting/Redeeming of xPOSITION, and the price difference between Anchor Price and Min Price exceeded **threshold**
* **Max** stETH/USD **Price** is used while Redeeming fxUSD, and the price difference between Anchor Price and Max Price **didn't** exceed **threshold**
* **Anchor Price** is used while Redeeming fxUSD, and the price difference between Anchor Price and Max Price exceeded **threshold**

\


