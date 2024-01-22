# Vaults

The daily farming yields in vaults automatically get bonded. Farmers earn more yields in ALD through the bonding process and can have this income auto compounded in the Staking Pool as well. This will significantly improve farmers’ APY and capital efficiency. The vaults are all quality strategies selected by the Boule Council.

The number of ALD bond obtained by farmers every day is calculated as follows:

Harvest once per epoch (6400 blocks), and automatically bond the farming yields minerProfit into ALD according to the ratio to be bonded expressed as $$BondPercent_{vault}$$. The ratio is 100% for now, the number of ALD that farmer i can get in each epoch is:

$$minerBondald_i= aldSupply((1+\cfrac{minerProfit_i*BondPercent_{vault}}{Reserve_{bond}})^{LR}-1)*Discount_{asset}$$

$$minerProfit_i$$ is farmer i’s total farming yield in the epoch. For example, farmer i gets 100 CRV and 50 LDO (CRV = $4 & LDO = $5) from staking stETH in the Convex vault for the epoch, then total farming yield is = $4_100 + $5_50= $650.

At the end of the epoch, the amount of ALD that farmer will receive is $$minerBondald_i$$, and is auto staked into the staking pool for compounding interests. When $$BondPercent_{vault}$$<100%, $$minerProfit_i*(1-BondPercent_{vault})$$ is no longer entering the Bond Pool, but pays back to farmers.

![](<../.gitbook/assets/image (80).png>)

Bonding profit will be transferred to the Treasury and POL Pool in proportion. For example, $$profitPOLPercent_{cry}=50\%$$, which means 50% of bonding profit will be stored in POL, which can be used to purchase ALD from the secondary market.
