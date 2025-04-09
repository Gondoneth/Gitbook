# asdPENDLE Vaults

**What is asdPENDLE**

asdPENDLE represents the compounding sdPENDLE in the StakeDAO PENDLE Locker. The total amount of asdPENDLE contained in the compounder is equal to the total sdPENDLE balance multiplied by the current index:

sdPENDLE\_Balance =asdPENDLE\_Balance \* Current\_asdPENDLE\_Index

Using asdPENDLE to represent a share of the underlying compounding sdPENDLE vault simplifies the smart contracts and is more gas efficient.

The asdPENDLE compounder has been upgraded and is now fully liquid, allowing instant withdrawals and further integrations with money market protocols.

**What is veSDT delegate**

By delegating veSDT to asdPENDLE vault, users’ sdPENDLE reward will be boosted up to 2.5X. Besides, veSDT delegators can share 10% of sdPENDLE’s bribe rewards.

**Is it safe?**&#x20;

The concentrator is built by the experienced and security-obsessed AladdinDAO team, and it is audited by SECBIT Labs. Check out the audit here.

[SECBIT](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/audit-reports/SECBIT_Concentrator_asdPENDLE_v1.0_20240813.pdf)

**How much does it cost?**

Concentrator takes a 10% treasury fee and a 2% harvest fee on yields. The fees were collected during the harvest process and distributed to the Treasury and Keeper respectively.
