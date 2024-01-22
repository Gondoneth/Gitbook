# aCVX Vaults

**What is aCVX**

aCVX simply represents the compounding CVX in the Concentrator vault. The total amount of CVX contained in the Concentrator vault is equal to the total aCVX balance multiplied by the current index:

CVX\_Balance = aCVX\_Balance \* Current\_aCVX\_Index

Using aCVX to represent a share of the underlying compounding CVX vault simplifies the smart contracts and is more gas efficient.



**Is it safe?**\
The concentrator is built by the experienced and security-obsessed AladdinDAO team, and it is audited by SECBIT Labs. Check out the audit here.

[SECBIT](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT\_Aladdin\_aCVX\_Report\_v1.0\_20231018.pdf)



**How much does it cost?**

Concentrator takes a 10% treasury fee and a 2% harvest fee on yields. The fees were collected during the harvest process and distributed to the Treasury and Keeper respectively.

<table><thead><tr><th width="223">Vaults</th><th>Treasury Fee</th><th>Harvest Fee</th></tr></thead><tbody><tr><td>aCVX Compounder</td><td>10.00%</td><td>2.00%</td></tr></tbody></table>



**Deployed Contracts?**

{% embed url="https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#concentrator-for-cvx" %}

