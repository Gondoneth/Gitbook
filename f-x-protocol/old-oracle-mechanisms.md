# Oracle

**stETH Oracle**

f(x) uses Chainlink 30 min TWAP stETH/USD for mint/redeem transactions under normal circumstances where ABS((Chainlink ETH/USD-stETH/USD)/stETH/USD) < 1% OR 99% < (Curve ETH/stETH) < 101%.

Otherwise, the system will do the followings to protect f(x) Protocol from stETH depegging risk:

1. f(x) mint transactions are disabled;
2. fETH redeem transactions will be done based on max (Chainlink ETH/USD, Chainlink stETH/USD, Curve stETH/USD);
3. xETH redeem transactions will be done based on min (Chainlink ETH/USD, Chainlink stETH/USD, Curve stETH/USD);
4. Curve stETH/USD is calculated as Curve stETH/ETH x Chainlink ETH/USD TWAP. Curve stETH/ETH is EMA price from stETH/ETH NG pool;
5. All Chainlink price feeds above are quoted as 30 min TWAP.\


**frxETH Oracle**

The price of frxETH is determined by Curve frxETH/ETH EMA Price\* Chainlink TWAP ETH/USD. If Curve frxETH/ETH EMA Price > 101% OR Curve frxETH/ETH EMA Price < 99%, it triggers a depegging process, and minting with it is (temporarily) disabled. However, redemptions remain enabled (as always), stable-side (fxUSD) redemptions use the higher of the two divergent prices (ETH or LSD), and leverage-side (xfrxETH) redemptions use the lower. When the peg normalizes, minting resumes. This mechanism ensures rUSD and xfrxETH token holders are protected, and no urgent action is ever needed in the event of a temperory depegging event.



**eETH Oracle**

For eETH, the price is based on Chainlink TWAP ETH/USD. If Curve weETH/ETH EMA Price >  101% OR Curve weETH/ETH EMA Price < 99%, it initiates a depegging process, and minting with it is (temporarily) disabled. However, redemptions remain enabled (as always), stable-side (rUSD) redemptions use the higher of the two divergent prices (ETH or LSD), and leverage-side (xeETH) redemptions use the lower. When the peg normalizes, minting resumes. This mechanism ensures rUSD and xeETH token holders are protected, and no urgent action is ever needed in the event of a temperory depegging event.



**ezETH Oracle**

For ezETH, the price is based on Chainlink TWAP ETH/USD. If Curve ezETH/ETH EMA Price >  101% OR Curve ezETH/ETH EMA Price < 99%, it initiates a depegging process, and minting with it is (temporarily) disabled. However, redemptions remain enabled (as always), stable-side (rUSD) redemptions use the higher of the two divergent prices (ETH or LSD), and leverage-side (xezETH) redemptions use the lower. When the peg normalizes, minting resumes. This mechanism ensures rUSD and xezETH token holders are protected, and no urgent action is ever needed in the event of a temperory depegging event.



WBTC Oracle

For WBTC, the price is based on Chainlink TWAP BTC/USD. If Curve WBTC/BTC EMA Price >  101% OR Curve WBTC/BTC EMA Price < 99%, it initiates a depegging process, and minting with it is (temporarily) disabled. However, redemptions remain enabled (as always), stable-side (btcUSD) redemptions use the higher of the two divergent prices (BTC or WBTC), and leverage-side (xWBTC) redemptions use the lower. When the peg normalizes, minting resumes. This mechanism ensures btcUSD and xWBTC token holders are protected, and no urgent action is ever needed in the event of a temperory depegging event.
