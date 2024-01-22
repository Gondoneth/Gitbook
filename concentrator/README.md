---
description: >-
  Concentrator by Aladdin DAO maximizes Convex APYs and earns yield in the best
  DeFi tokens
---

# Concentrator

![](<../.gitbook/assets/image (15).png>)

**What is Concentrator?**



Concentrator is a yield enhancer that boosts yields on Convex vaults by concentrating all rewards into auto-compounding top-tier tokens like aCRV (cvxCRV) and aFXS (cvxFXS).\


{% embed url="https://concentrator.aladdin.club/#/vault" %}

**Why use Concentrator?**



i. Set & forget to increase Convex yields by 20%+&#x20;

ii. Yields are concentrated into top-tier wrapped auto-compounding tokens (aCRV = cvxCRV, aFXS = cvxFXS), thus earning the most rewards denominated in the best tokens (farm & hold)&#x20;

iii. Claim your rewards at a time of your choosing



**How does it work?**



Users deposit Curve LP tokens or zap into their selected strategy. Funds are automatically staked in Convex vaults and rewards are periodically harvested. Harvested rewards are swapped to aCRV or aFXS, which are auto-compounding wrappers for cvxCRV and cvxFXS/FXS respectively.

Users may unwrap their aCRV or aFXS at any time, or zap out to blue chip assets.

<figure><img src="https://lh4.googleusercontent.com/LPyGBPor6N_y_6l6ARUb0HT3ysesNLZgtEvU36Byx3-359b-1pXm07IGfSBDZOTBrVSjoIlDXQheAOkPX-uvLRis0tH3gg5fEWMPb1kgfaatnPxqHxLyfWV8PznNL73sMVGiiSdGZ4fBXWFnkx_-o5DNnq7blX_HOpWkPGflaoPKaY5Qf3TYKwyY-Q" alt=""><figcaption></figcaption></figure>

**What is aCRV/aFXS?**



aCRV and aFXS are each wrappers representing a share of an auto-compounding Concentrator vault. Each one is backed by a different farming strategy. All farming yields for each strategy are compounded back into more of the underlying token.

| **Auto-compounding Token** | **Underlying (Wrapped) Token** | **Farming Strategy**  |
| -------------------------- | ------------------------------ | --------------------- |
| aCRV                       | cvxCRV                         | Convex cvxCRV staking |
| aFXS                       | cvxFXS                         | cvxFXS Staking        |

The total amount of underlying token contained in the auto-compounding Concentrator vault is equal to the total Auto-compounding token balance multiplied by the current index:



cvxCRV\_Balance = aCRV\_Balance \* Current\_aCRV\_Index&#x20;

cvxFXS\_Balance = aFXS\_Balance \* Current\_aFXS\_Index



Using aCRV/aFXS to represent a share of the underlying compounding cvxCRV vault simplifies the smart contracts and is more gas efficient, and it creates a simple, single, bridgeable token representing an increasing amount of the underlying.



**How much does it cost?**



Concentrator takes a 10% treasury fee and a 2% harvest fee on yields. The fees were collected during the harvest process and distributed to the Treasury and Keeper respectively.



**What is aCRV/aFXS contract address?**



<table><thead><tr><th>Chains</th><th>CRV Address</th><th>aCRV Address</th><th data-hidden></th></tr></thead><tbody><tr><td>Ethereum</td><td>0xD533a949740bb3306d119CC777fa900bA034cd52</td><td>0x2b95A1Dcc3D405535f9ed33c219ab38E8d7e0884</td><td></td></tr><tr><td>Arbitrum</td><td>0x11cdb42b0eb46d95f990bedd4695a6e3fa034978</td><td>0xebf1f92d4384118bfb91b4496660a95931c92861</td><td></td></tr><tr><td>Polygon</td><td>0x172370d5cd63279efa6d502dab29171933a610af</td><td>0x89c90e480a39fbe3886bb5bd53ba5b1acc69d4fb</td><td></td></tr><tr><td>Fantom</td><td>0x1e4f97b9f9f913c46f1632781732927b9019c68b</td><td>0x666a3776b3e82f171cb1dff7428b6808d2cd7d02</td><td></td></tr></tbody></table>



| Chains   | FXS Address                                | aFXS Address                               |
| -------- | ------------------------------------------ | ------------------------------------------ |
| Ethereum | 0x3432B6A60D23Ca0dFCa7761B7ab56459D9C964D0 | 0xDAF03D70Fe637b91bA6E521A32E1Fb39256d3EC9 |
