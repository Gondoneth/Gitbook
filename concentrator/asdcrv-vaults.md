# asdCRV Vaults

**What is asdCRV**

asdCRV simply represents the compounding sdCRV in the StakeDAO CRV Locker. The total amount of asdCRV contained in the compounder is equal to the total sdCRV balance multiplied by the current index:

asdCRV\_Balance =sdCRV\_Balance \* Current\_sdCRV\_Index

Using asdCRV to represent a share of the underlying compounding sdCRV vault simplifies the smart contracts and is more gas efficient.

\
The asdCRV compounder has been upgraded and is now fully liquid, which allows for instant withdrawals and further integrations with money market protocols.



**What is veSDT delegate**

By delegating veSDT to asdCRV vault, users’ asdCRV reward will be boosted up to 2.5X. Besides, veSDT delegators are entitled to share 10% of sdCRV’s bribe rewards.



**Is it safe?**\
The concentrator is built by the experienced and security-obsessed AladdinDAO team, and it is audited by SECBIT Labs. Check out the audit here.

[SECBIT](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_sdCRV\_Report\_v1.0\_20230202.pdf)



**How much does it cost?**

Concentrator takes a 10% treasury fee and a 2% harvest fee on yields. The fees were collected during the harvest process and distributed to the Treasury and Keeper respectively.



<table><thead><tr><th width="84">PID</th><th>Name</th><th>Harvest Fee</th><th>Treasury Fee</th><th>Boost Fee</th><th data-hidden align="center">Underlying</th><th data-hidden align="center">Strategy</th><th data-hidden>Notes</th></tr></thead><tbody><tr><td></td><td>asdCRV Compounder</td><td>0.50%</td><td>10.00%</td><td>10.00%</td><td align="center"></td><td align="center"></td><td></td></tr><tr><td>0</td><td>MIM+3CRV</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x5a6A4D54456819380173272A5E8E9B9904BdF41B</td><td align="center">0x3125FC8b81593B39baC2590C58c48CB417e5D859</td><td></td></tr><tr><td>1</td><td>ETH+pETH</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x9848482da3Ee3076165ce6497eDA906E66bB85C5</td><td align="center">0xB634b550BE88c968e21DCBC68BCb96D39F75B06C</td><td></td></tr><tr><td>2</td><td>clevUSD+FRAXBP</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x84c333e94aea4a51a21f6cf0c7f528c50dc7592c</td><td align="center">0x6deaF124A8bFb8616B994B4fD55544A68062C274</td><td></td></tr><tr><td>3</td><td>CRV+cvxCRV</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x971add32Ea87f10bD192671630be3BE8A11b8623</td><td align="center">0x4cDB0e8CEC25d134948F5c26395B529D0F17042D</td><td></td></tr><tr><td>4</td><td>eCFX+ETH</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x8C88538688aca3b733aD08b12BEe4574c0C00907</td><td align="center">0xEb6Bcc57dF50F007Da79c12CC1790153CC3352ec</td><td></td></tr><tr><td>5</td><td>USDT+crvUSD</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x390f3595bCa2Df7d23783dFd126427CCeb997BF4</td><td align="center">0x44d5c2Ad61cfa4d01D79ef11b4feE6C9d6616Ba6</td><td></td></tr><tr><td>6</td><td>USDC+crvUSD</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x4DEcE678ceceb27446b35C672dC7d61F30bAD69E</td><td align="center">0xE1c863E0Bb81717dEa24a477eC23AD8602340198</td><td></td></tr><tr><td>7</td><td>USDC/WBTC/ETH</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0x7f86bf177dd4f3494b841a37e810a34dd56c829b</td><td align="center">0x297DB2492E7B26CC800C6e4a5ebf4FA84ff53aA3</td><td></td></tr><tr><td>8</td><td>USDT/WBTC/ETH</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0xf5f5b97624542d72a9e06f04804bf81baa15e2b4</td><td align="center">0xF01Bd63cAB35e9D7EfC0e3684bDda33D49EdA51f</td><td></td></tr><tr><td>9</td><td>CRV+sdCRV</td><td>2.00%</td><td>10.00%</td><td></td><td align="center">0xCA0253A98D16e9C1e3614caFDA19318EE69772D0</td><td align="center">0x4e5854A9fB8CBE4f9196D30dE5014FCe9699295c</td><td></td></tr></tbody></table>

**Concentrator Github?**

{% @github-files/github-code-block url="https://github.com/AladdinDAO/aladdin-v3-contracts/tree/main/contracts/concentrator/stakedao" %}

**Deployed Contracts?**



{% @github-files/github-code-block url="https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#concentrator-for-sdcrv" %}
