# aCRV(IFO) Vaults

**IFO?**\
Initial Farm Offering. A new and fair way to democratize ownership of Concentrator and raise some aCRV funds for Concentrator treasury. Deposit your Curve LPs to Concentrator’s IFO vaults just like a regular Concentrator vault, except your yields are automatically exchanged for CTR tokens. 1 aCRV yield harvested = 1 CTR reward.

{% embed url="https://concentrator.aladdin.club/" %}

\
**How long does it run?**

We are raising 2.5m aCRV for 50% of the FDV token allocation. The IFO vaults will continue distributing CTR tokens until we reach 2.5m aCRV harvested. Afterwards vaults automatically revert to earning regular aCRV returns!



**So I give up my aCRV yields and receive CTR instead.  Why would I do that?**

CTR is Concentrator’s token, and it is designed to be a cash(flow) cow. CTR uses the Curve ve-lock mechanism, and veCTR holders will vote to allocate/receive up to 50% of the platform’s revenue denominated in aCRV (auto-compounding cvxCRV). veCTR holders also, of course, receive governance rights. CTR has a very [favourable emission schedule](https://medium.com/@0xconcentrator\_29486/find-your-future-in-a-farm-9e571934c32c). There will be no CTR emissions after the end of the IFO (no liquidity mining, no new minting), so no inflation.

\
**Can I participate in the IFO using my aCRV?**\
The IFO vaults only accept Curve LP tokens, not aCRV directly.  However, aCRV can be used to farm CTR by providing liquidity in the [Balancer IFO Liquidity Pool for aCRV-CTR](https://app.balancer.fi/#/pool/0x80a8ea2f9ebfc2db9a093bd46e01471267914e490002000000000000000002a2).  Alternatively, withdraw your cvxCRV and zap it into the cvxCRV/CRV Concentrator vault.  Both of those options allow you to stay mostly exposed to aCRV.\
\
**Where can I swap CTR?**

There is a [liquidity pool on Balancer](https://app.balancer.fi/#/pool/0x80a8ea2f9ebfc2db9a093bd46e01471267914e490002000000000000000002a2) where CTR can be exchanged for aCRV.  This pool is a weighted pool skewed heavily to aCRV, so watch out for slippage on CTR swaps!



**Why the unusual weighted Balancer liquidity pool?  Why not just Curve v2/Uni?**

Neither Curve nor Uni offer fixed weight pools.  The [weighted Balancer pool](https://docs.balancer.fi/products/balancer-pools/weighted-pools) skewed heavily to aCRV will allow LPs to provide CTR liquidity while taking on very little impermanent loss compared to just holding aCRV, making LPing in this pool a much less risky option for farming CTR. An interesting side-effect is that bigger buys and sells of the token with the small weight will suffer more slippage in the weighted liquidity pool, and so large scale mercenary farm-and-dump outfits may be less inclined to exploit this launch and dump token price.\
\
After the IFO is over and all the CTR has been emitted, CTR farming rewards in the Balancer pool will be **discontinued**.

\
**What makes the Concentrator IFO more fair than other token launches?**\
Two things:

1. The price. Everybody farming gets 1 CTR for 1 aCRV, no matter how big your deposit is. No tokens have ever been sold to anyone for less.
2. The distribution schedule. No pre-sold tokens and no vesting allotments means no unlock bomb in the future.\


**Why are you raising funds for Concentrator?**

Glad you asked, anon!  The aCRV that Concentrator raises are going to be used to improve aCRV liquidity, especially on non-mainnet chains.  Curve is emitting CRV on many chains now but most of the yield opportunities for CRV still live on mainnet.  aCRV will provide a simple option to help CRV holders on other chains like Arbitrum, Avalanche, Optimism, etc to earn yields. \


**Is there any way to earn CTR other than farming the IFO?**

Yes!  There is a token allocation that will be distributed to the community by veCTR vote called the Community Booster allocation.  People in the community who help to spread Concentrator’s message or otherwise help out during the IFO can be nominated to be on the ballot.  See more details [here](https://medium.com/@0xconcentrator\_29486/lets-concentrate-together-19e575520640).\
\
Additionally a small airdrop of CTR will be issued to the earliest users of Concentrator.

&#x20;

**I’m a member of the AladdinDAO community and hold (x)ALD.  Do I receive CTR?**

AladdinDAO will receive 30% of the CTR tokens.  Aladdin will instantly lock that entire allocation for the maximum duration (4 years) and continually re-lock those tokens.  xALD holders will vote to direct the veCTR governance power held by Aladdin, and any revenue earned by the Aladdin veCTR tokens will be directly claimable by ALD stakers. (We may revamp Aladdin tokenomics at some point).





**Fees**

<table><thead><tr><th width="82">PID</th><th>Name</th><th>Harvest Fee</th><th>Treasury Fee</th><th data-hidden align="center">Underlying</th><th data-hidden>Notes</th></tr></thead><tbody><tr><td></td><td>aCRV Compounder</td><td>2.00%</td><td>10.00%</td><td align="center"></td><td></td></tr><tr><td>0</td><td>ETH+stETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x06325440D014e39736583c165C2963BA99fAf14E</td><td></td></tr><tr><td>1</td><td>FRAX+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B</td><td></td></tr><tr><td>2</td><td>USDT+WBTC+WETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xc4AD29ba4B3c580e6D59105FFf484999997675Ff</td><td></td></tr><tr><td>3</td><td>CRV+cvxCRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x9D0464996170c6B9e75eED71c68B99dDEDf279e8</td><td>deprecated</td></tr><tr><td>4</td><td>ETH+CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xEd4064f376cB8d68F770FB1Ff088a3d0F3FF5c4d</td><td></td></tr><tr><td>5</td><td>ETH+CVX</td><td>2.00%</td><td>10.00%</td><td align="center">0x3A283D9c08E8b55966afb64C515f5143cf907611</td><td></td></tr><tr><td>6</td><td>FXS+cvxFXS</td><td>2.00%</td><td>10.00%</td><td align="center">0xF3A43307DcAFa93275993862Aae628fCB50dC768</td><td></td></tr><tr><td>7</td><td>DAI+USDC+USDT</td><td>2.00%</td><td>10.00%</td><td align="center">0x6c3F90f043a72FA612cbac8115EE7e52BDe6E490</td><td></td></tr><tr><td>8</td><td>iDAI+iUSDC+iUSDT</td><td>2.00%</td><td>10.00%</td><td align="center">0x5282a4eF67D9C33135340fB3289cc1711c13638C</td><td>deprecated</td></tr><tr><td>9</td><td>MIM+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x5a6A4D54456819380173272A5E8E9B9904BdF41B</td><td></td></tr><tr><td>10</td><td>renBTC+WBTC</td><td>2.00%</td><td>10.00%</td><td align="center">0x49849C98ae39Fff122806C06791Fa73784FB3675</td><td>deprecated</td></tr><tr><td>11</td><td>PUSd+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x8EE017541375F6Bcd802ba119bdDC94dad6911A1</td><td></td></tr><tr><td>12</td><td>DAI+USDC+USDT+sUSD</td><td>2.00%</td><td>10.00%</td><td align="center">0xC25a3A3b969415c80451098fa907EC722572917F</td><td></td></tr><tr><td>13</td><td>renBTC+WBTC+sBTC</td><td>2.00%</td><td>10.00%</td><td align="center">0x075b1bb99792c9E1041bA13afEf80C91a1e70fB3</td><td>deprecated</td></tr><tr><td>14</td><td>ETH+sETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xA3D87FffcE63B53E0d54fAa1cc983B7eB0b74A9c</td><td></td></tr><tr><td>15</td><td>FRAX+USDC</td><td>2.00%</td><td>10.00%</td><td align="center">0x3175Df0976dFA876431C2E9eE6Bc45b65d3473CC</td><td></td></tr><tr><td>16</td><td>FRAX+FPI</td><td>2.00%</td><td>10.00%</td><td align="center">0x4704aB1fb693ce163F7c9D3A31b3FF4eaF797714</td><td></td></tr><tr><td>17</td><td>alUSD+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x43b4FdFD4Ff969587185cDB6f0BD875c5Fc83f8c</td><td></td></tr><tr><td>18</td><td>cDAI+cUSDC</td><td>2.00%</td><td>10.00%</td><td align="center">0x845838DF265Dcd2c412A1Dc9e959c7d08537f8a2</td><td>deprecated</td></tr><tr><td>19</td><td>dola+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xAA5A67c256e27A5d80712c51971408db3370927D</td><td>deprecated</td></tr><tr><td>20</td><td>BUSD+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x4807862AA8b2bF68830e4C8dc86D0e9A998e085a</td><td>deprecated</td></tr><tr><td>21</td><td>ETH+alETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xC4C319E2D4d66CcA4464C0c2B32c9Bd23ebe784e</td><td></td></tr><tr><td>22</td><td>agEUR+EURT+EURS</td><td>2.00%</td><td>10.00%</td><td align="center">0xb9446c4Ef5EBE66268dA6700D26f96273DE3d571</td><td></td></tr><tr><td>23</td><td>LUSD+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xEd279fDD11cA84bEef15AF5D39BB4d4bEE23F0cA</td><td></td></tr><tr><td>24</td><td>Silo+FRAX</td><td>2.00%</td><td>10.00%</td><td align="center">0x2302aaBe69e6E7A1b0Aa23aAC68fcCB8A4D2B460</td><td></td></tr><tr><td>25</td><td>TUSD+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xEcd5e75AFb02eFa118AF914515D6521aaBd189F1</td><td></td></tr><tr><td>26</td><td>sUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0xe3c190c57b5959Ae62EfE3B6797058B76bA2f5eF</td><td></td></tr><tr><td>27</td><td>BUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x8fdb0bB9365a46B145Db80D0B1C5C5e979C84190</td><td></td></tr><tr><td>28</td><td>alUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0xB30dA2376F63De30b42dC055C93fa474F31330A5</td><td></td></tr><tr><td>29</td><td>TUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x33baeDa08b8afACc4d3d07cf31d49FC1F1f3E893</td><td></td></tr><tr><td>30</td><td>LUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x497CE58F34605B9944E6b15EcafE6b001206fd25</td><td></td></tr><tr><td>31</td><td>ETH+pETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x9848482da3Ee3076165ce6497eDA906E66bB85C5</td><td></td></tr><tr><td>32</td><td>ETH+cbETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x5b6C539b224014A09B3388e51CaAA8e354c959C8</td><td></td></tr><tr><td>33</td><td>ETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xf43211935C781D5ca1a41d2041F397B8A7366C7A</td><td></td></tr><tr><td>34</td><td>bLUSD+LUSD3CRV-f</td><td>2.00%</td><td>10.00%</td><td align="center">0x5ca0313d44551e32e0d7a298ec024321c4bc59b4</td><td></td></tr><tr><td>35</td><td>WBTC+sBTC</td><td>2.00%</td><td>10.00%</td><td align="center">0x051d7e5609917Bd9b73f04BAc0DED8Dd46a74301</td><td></td></tr><tr><td>36</td><td>multiBTC+crvWSBTC</td><td>2.00%</td><td>10.00%</td><td align="center">0x2863a328A0B7fC6040f11614FA0728587DB8e353</td><td></td></tr><tr><td>37</td><td>clevCVX+CVX</td><td>2.00%</td><td>10.00%</td><td align="center">0xf9078fb962a7d13f55d40d49c8aa6472abd1a5a6</td><td></td></tr><tr><td>38</td><td>clevUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x84c333e94aea4a51a21f6cf0c7f528c50dc7592c</td><td></td></tr><tr><td>39</td><td>ETH+CLEV</td><td>2.00%</td><td>10.00%</td><td align="center">0x6c280db098db673d30d5b34ec04b6387185d3620</td><td></td></tr><tr><td>40</td><td>ETH+rETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x6c38ce8984a890f5e46e6df6117c26b3f1ecfc9c</td><td></td></tr><tr><td>41</td><td>GEAR+ETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x5be6c45e2d074faa20700c49ada3e88a1cc0025d</td><td></td></tr><tr><td>42</td><td>WETH+stETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x828b154032950c8ff7cf8085d841723db2696056</td><td></td></tr><tr><td>43</td><td>STG+USDC</td><td>2.00%</td><td>10.00%</td><td align="center">0xdf55670e27be5cde7228dd0a6849181891c9eba1</td><td></td></tr><tr><td>44</td><td>ETH+LDO</td><td>2.00%</td><td>10.00%</td><td align="center">0xb79565c01b7ae53618d9b847b9443aaf4f9011e7</td><td></td></tr><tr><td>45</td><td>ETH+MATIC</td><td>2.00%</td><td>10.00%</td><td align="center">0xd8eb58d76af99547333cfeeb6a0f9bd1a63b6492</td><td></td></tr><tr><td>46</td><td>ETH+CNC</td><td>2.00%</td><td>10.00%</td><td align="center">0xf9835375f6b268743ea0a54d742aa156947f8c06</td><td></td></tr><tr><td>47</td><td>tBTC+crvWSBTC</td><td>2.00%</td><td>10.00%</td><td align="center">0xf95aaa7ebb1620e46221b73588502960ef63dba0</td><td></td></tr><tr><td>48</td><td>ETH+CTR</td><td>2.00%</td><td>10.00%</td><td align="center">0x3f0e7916681452d23cd36b1281457da721f2e5df</td><td></td></tr><tr><td>49</td><td>USDP+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xc270b3B858c335B6BA5D5b10e2Da8a09976005ad</td><td></td></tr><tr><td>50</td><td>CRV+cvxCRV</td><td>2.00%</td><td>10.00%</td><td align="center">0x971add32Ea87f10bD192671630be3BE8A11b8623</td><td></td></tr><tr><td>51</td><td>eCFX+ETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x8C88538688aca3b733aD08b12BEe4574c0C00907</td><td></td></tr><tr><td>52</td><td>rETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xbA6c373992AD8ec1f7520E5878E5540Eb36DeBf1</td><td></td></tr><tr><td>53</td><td>stETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x4d9f9D15101EEC665F77210cB999639f760F831E</td><td></td></tr><tr><td>54</td><td>cbETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x548E063CE6F3BaC31457E4f5b4e2345286274257</td><td></td></tr><tr><td>55</td><td>sETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x663aC72a1c3E1C4186CD3dCb184f216291F4878C</td><td></td></tr><tr><td>56</td><td>FRAX+USDP</td><td>2.00%</td><td>10.00%</td><td align="center">0xFC2838a17D8e8B1D5456E0a351B0708a09211147</td><td></td></tr><tr><td>57</td><td>UZD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x68934F60758243eafAf4D2cFeD27BF8010bede3a</td><td></td></tr><tr><td>58</td><td>ETH+wBETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xBfAb6FA95E0091ed66058ad493189D2cB29385E6</td><td></td></tr><tr><td>59</td><td>USDT+crvUSD</td><td>2.00%</td><td>10.00%</td><td align="center">0x390f3595bCa2Df7d23783dFd126427CCeb997BF4</td><td></td></tr><tr><td>60</td><td>USDP+crvUSD</td><td>2.00%</td><td>10.00%</td><td align="center">0xCa978A0528116DDA3cbA9ACD3e68bc6191CA53D0</td><td></td></tr><tr><td>61</td><td>TUSD+crvUSD</td><td>2.00%</td><td>10.00%</td><td align="center">0x34D655069F4cAc1547E4C8cA284FfFF5ad4A8db0</td><td></td></tr><tr><td>62</td><td>USDC+crvUSD</td><td>2.00%</td><td>10.00%</td><td align="center">0x4DEcE678ceceb27446b35C672dC7d61F30bAD69E</td><td></td></tr><tr><td>63</td><td>USDC/WBTC/ETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x7f86bf177dd4f3494b841a37e810a34dd56c829b</td><td></td></tr><tr><td>64</td><td>USDT/WBTC/ETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xf5f5b97624542d72a9e06f04804bf81baa15e2b4</td><td></td></tr><tr><td>65</td><td>ETH/stETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x21e27a5e5513d6e65c4f830167390997aa84843a</td><td></td></tr></tbody></table>





**Where can I get more details?**\
\
Check out the launch article [here](https://medium.com/@0xconcentrator\_29486/find-your-future-in-a-farm-9e571934c32c).



**Is it safe?**

\
The concentrator is built by the experienced and security-obsessed AladdinDAO team, and it is audited by SECBIT Labs. Check out the audit here.

[PeckShield](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/PeckShield-Audit-Report-AladdinDAO-Concentrator-v1.0-20220704.pdf)

[SECBIT](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_Concentrator\_IFO\_Report\_v1.2\_20220701.pdf)



**Concentrator Github?**

[**https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#concentrator**](https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#concentrator)

**Concentrator** Governance Multisig

Concentrator Treasury: [0xA0FB1b11ccA5871fb0225B64308e249B97804E99](https://etherscan.io/address/0xA0FB1b11ccA5871fb0225B64308e249B97804E99)



