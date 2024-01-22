# aFXS Vaults

**What is aFXS**

aFXS simply represents the compounding cvxFXS in the Concentrator vault. The total amount of cvxFXS contained in the Concentrator vault is equal to the total aFXS balance multiplied by the current index:

cvxFXS\_Balance = aFXS\_Balance \* Current\_aFXS\_Index

Using aFXS to represent a share of the underlying compounding cvxFXS vault simplifies the smart contracts and is more gas efficient.



**Is it safe?**\
The concentrator is built by the experienced and security-obsessed AladdinDAO team, and it is audited by SECBIT Labs. Check out the audit here.

[SECBIT](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_AladdinDAO\_aFXS\_Report.pdf)



**How much does it cost?**

Concentrator takes a 10% treasury fee and a 2% harvest fee on yields. The fees were collected during the harvest process and distributed to the Treasury and Keeper respectively.



<table><thead><tr><th width="85">PID</th><th>Name</th><th>Harvest Fee</th><th>Treasury Fee</th><th data-hidden align="center">Underlying</th><th data-hidden>Notes</th></tr></thead><tbody><tr><td></td><td>aFXS Compounder</td><td>2.00%</td><td>10.00%</td><td align="center"></td><td></td></tr><tr><td>0</td><td>FRAX+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xd632f22692FaC7611d2AA1C0D552930D43CAEd3B</td><td></td></tr><tr><td>1</td><td>FXS+cvxFXS</td><td>2.00%</td><td>10.00%</td><td align="center">0xF3A43307DcAFa93275993862Aae628fCB50dC768</td><td>deprecated</td></tr><tr><td>2</td><td>FRAX+USDC</td><td>2.00%</td><td>10.00%</td><td align="center">0x3175Df0976dFA876431C2E9eE6Bc45b65d3473CC</td><td></td></tr><tr><td>3</td><td>sUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0xe3c190c57b5959Ae62EfE3B6797058B76bA2f5eF</td><td></td></tr><tr><td>4</td><td>TUSD+3CRV</td><td>2.00%</td><td>10.00%</td><td align="center">0xEcd5e75AFb02eFa118AF914515D6521aaBd189F1</td><td></td></tr><tr><td>5</td><td>BUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x8fdb0bB9365a46B145Db80D0B1C5C5e979C84190</td><td></td></tr><tr><td>6</td><td>alUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0xB30dA2376F63De30b42dC055C93fa474F31330A5</td><td></td></tr><tr><td>7</td><td>Silo+FRAX</td><td>2.00%</td><td>10.00%</td><td align="center">0x2302aaBe69e6E7A1b0Aa23aAC68fcCB8A4D2B460</td><td></td></tr><tr><td>8</td><td>TUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x33baeDa08b8afACc4d3d07cf31d49FC1F1f3E893</td><td></td></tr><tr><td>9</td><td>ETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xf43211935C781D5ca1a41d2041F397B8A7366C7A</td><td></td></tr><tr><td>10</td><td>clevUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td align="center">0x84c333e94aea4a51a21f6cf0c7f528c50dc7592c</td><td></td></tr><tr><td>11</td><td>ETH+CLEV</td><td>2.00%</td><td>10.00%</td><td align="center">0x6c280db098db673d30d5b34ec04b6387185d3620</td><td></td></tr><tr><td>12</td><td>FPIS+cvxFPIS</td><td>2.00%</td><td>10.00%</td><td align="center">0xfBB481A443382416357fA81F16dB5A725DC6ceC8</td><td></td></tr><tr><td>13</td><td>rETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0xbA6c373992AD8ec1f7520E5878E5540Eb36DeBf1</td><td></td></tr><tr><td>14</td><td>stETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x4d9f9D15101EEC665F77210cB999639f760F831E</td><td></td></tr><tr><td>15</td><td>cbETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x548E063CE6F3BaC31457E4f5b4e2345286274257</td><td></td></tr><tr><td>16</td><td>sETH+frxETH</td><td>2.00%</td><td>10.00%</td><td align="center">0x663aC72a1c3E1C4186CD3dCb184f216291F4878C</td><td></td></tr><tr><td>17</td><td>FRAX+USDP</td><td>2.00%</td><td>10.00%</td><td align="center">0xFC2838a17D8e8B1D5456E0a351B0708a09211147</td><td></td></tr></tbody></table>

\
\


**Concentrator Github?**

{% embed url="https://github.com/AladdinDAO/aladdin-v3-contracts/tree/main/contracts/concentrator/fxs" %}

**Deployed Contracts?**

{% embed url="https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#concentrator-for-curve-fxscvxfxs-lp" %}

