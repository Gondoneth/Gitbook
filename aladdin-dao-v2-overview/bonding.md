# Bonding

Bonding is the core strategy of AladdinDAO’s New Tokenomics. Bonding is the optimal strategy to obtain ALD, because it is allocated on demand instead of the traditional DeFi block mining tokenomics. This model makes ALD an “on-demand supply” token, and also provides an alternative way to get ALD with a discount price compared to the secondary market.



There are 3 ways to bond:

1. Bond can be purchased directly with bluechip assets like ETH, WBTC, Dai, USDC, etc;
2. Bond with the LP tokens of ALD/ETH and ALD/USDC pools from Uniswap.
3. Vaults’ farming yields are automatically bonded;

The price of a bond does not depend on the secondary market but is automatically priced by an algorithm. The calculation formula is as follows:

&#x20;                                             $$aldBondPrice = \cfrac{Reserve_{bond}}{aldSupply*LR}$$

$$Reserve_{bond}$$ represents the value of Bond Treasury, including  $$Reserve_{Vaultbond}$$, $$Reserve_{UnderlyingBond}$$ **,** $$Reserve_{LP Bond}$$(ALD value excluded). $$aldSupply$$ represents the total supply of ALD. LR represents the asset-liability ratio, with an equation $$LR = \cfrac{Reserve_{bond}}{aldSupplyValue}$$where the denominator stands for the total value of ALD supply.

With the given LR value, the quantity of ALD Bond obtained from the bonding transaction is:

&#x20;                       $$Bondald=aldSupply((1+\cfrac{BondValue_{asset}}{Reserve_{bond}})^{LR}-1)*Discount_{asset}$$

$$Discount_{asset}$$ is the discount rate of bonding assets. It is used to adjust the proportion of various reserve assets in the reserve fund.

Once bonding is finished:

1. $$BondValue_{asset}$$ will be stored in treasury
2.  $$Bondald$$ will enter Staking Pool automatically, release linearly in 32k blocks.

    The graph below shows the complete process of bonding

![](<../.gitbook/assets/image (22).png>)

Bonding is automatically priced with the above algorithm. It can be predicted that when bonding happens, $$Reserve_{bond}$$ increases and $$aldBondPrice$$ will gradually increase too. The bond will have no price advantage when its price exceeds the secondary market price. Due to the increase of Reserve, the value of ALD will theoretically also increase. As a result of ALD price increases, the demand for bonds should grow as well, which will encourage more users to buy ALD through the bonding process. Hence, as the Reserve increases, ALD enters a benign mode of gradual appreciation.

When the secondary market does not correctly reflect the value of ALD and even drops below the bond price, users have no incentives to bond and Reserve will stop growing. At this time, the staking strategy will play a role, with continued expansion of ALD supply through the rebase process, $$aldBondPrice$$ will drop. As ALD supply gets larger, this may put pressure on ALD secondary market price as well, however this can be offset as value creation and demand continue to build up for ALD. In addition the POL pool will help to absorb selling pressure and reduce supply of ALD when secondary market price underperforms. Bonding will become attractive again at some point where $$aldBondPrice$$ is lower than ALD secondary market price.

The unique bond pricing algorithm makes ALD the first token based on a basket of reserve assets. The value of ALD increases as the community continues to build up the Reserve, which in turn maximizes the value of all ALD token holders and the entire Aladdin community.

The equivalent amount of tokens as bond sales are minted for reserve. 5% is allocated to ALDDAO holders (early backers and contributors) and 95% is reserved for boule/boule plus/talent hunter incentives. For this 95%, if the tokens are not used for the epoch, they can be burnt.

