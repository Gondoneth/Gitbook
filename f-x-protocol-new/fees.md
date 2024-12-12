# Fees

The protocol's revenue sources include Trading fees(Mint/Redeem xPOSITION fee, Rebalance fee, Liquidation fee, Redeem fee), Funding fees (charged during fxUSD depeg), and LSD yields from Basetokens.



Trading Fees

open/close xPOSITION fees

* Mint/Redeem xPOSITION Fee is set as 0.1% in default
* Minting of xPOSITION is floating by multiplying the default number 0.1% with a **Ratio**, for each **Step = 5%(Step is a Parameter which can be changed in future governance voting)** increase in AAVE V3 USDC Interest Rate, **Ratio** increased by 1:

<table><thead><tr><th width="164">Step</th><th width="506">AAVE V3 USDC Interest Interval</th><th>Ratio</th></tr></thead><tbody><tr><td>5%</td><td>0% - 10%</td><td>1.00</td></tr><tr><td></td><td>10% - 15%</td><td>2.00</td></tr><tr><td></td><td>15% - 20%</td><td>3.00</td></tr><tr><td></td><td>20% - 25%</td><td>4.00</td></tr><tr><td></td><td>25% - 30%</td><td>5.00</td></tr><tr><td></td><td>...</td><td>...</td></tr></tbody></table>

* Rebalance fee = Rebalance Bounty\*10%, Rebalance Bounty=Rebalance amount\*Rebalance penalty, Rebalance penalty is set to default as 2.5%
* Liquidation fee = Liquidation Bounty\*10%, Liquidation Bounty=Liquidation amount\*Liquidation penalty, Liquidation penalty TBD
* Redeem fee = Redeem amount\*0.5%

### Funding Fees

* When fxUSD is pegged, no funding fee is charged
* During fxUSD depegs, a funding fee is charged on each transaction. The peg status is determined by checking whether the EMA price of fxUSD/USDC in the secondary market deviates from the threshold, which is set to 0.5% by default.
*   The funding rate is calculated as:\
    **interest\_funding = interest\_usdc\_aave × Ratio\_funding**,\
    where **Ratio\_funding** is an exchangeable parameter (default value is 1) and **interest\_usdc\_aave** is the AAVE rate recorded at the last transaction.

    The funding fee formula is:\
    **Funding fee = n × interest\_funding × Period**,\
    where **n** is the amount of LSD held in the user's position, **Period = current time - last time**, with **last time** being the previous charge time and **current time** being the current charge time.

### Revenue Distribution

* **Trading Fees**: By default, 70% is allocated to the fxUSD Rebalance Pool (V2).
* **Funding Fees**: By default, 100% is allocated to the fxUSD Rebalance Pool (V2).
* **LSD Yields**: By default, 100% is allocated to the fxUSD Rebalance Pool (V2).

The above allocations can be adjusted through governance.



