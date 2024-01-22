---
description: Harvester
---

# Harvester

## Change the vault harvesting mechanism and remove withdrawal fees

Only addresses that meet the following two criteria are allowed to harvest:

* The addresses must hold at least 2500 veCTR
* The _ve_ holding period is at least 1 year from the harvest block

{% embed url="https://snapshot.org/#/concentratordao.eth/proposal/0xa263531cd6f948612d9596a16e7ef477058de9a8b8f4fc895b8325733adafc68" %}

## Concentrator Upgraded Contract

Harvster address= 0xfa86aa141e45da5183B42792d99Dede3D26Ec515

### Compounder Contract

aCRV = 0x2b95A1Dcc3D405535f9ed33c219ab38E8d7e0884

aFXS = 0xDAF03D70Fe637b91bA6E521A32E1Fb39256d3EC9

afrxETH = 0xb15Ad6113264094Fd9BF2238729410A07EBE5ABa

abcCVX = 0xDEC800C2b17c9673570FDF54450dc1bd79c8E359

asdCRV = 0x43E54C2E7b3e294De3A155785F52AB49d87B9922

### Harvester Contract

aCRVVault = 0xc8fF37F7d057dF1BB9Ad681b53Fa4726f268E0e8

aFXSVault = 0xD6E3BB7b1D6Fa75A71d48CFB10096d59ABbf99E1

afrxETHVault = 0x50B47c4A642231dbe0B411a0B2FBC1EBD129346D

\
Harvester ABI
-------------

{% embed url="https://louper.dev/diamond/0xfa86aa141e45da5183B42792d99Dede3D26Ec515?network=mainnet" %}

### Compounder harvest

1\. const amount =aToken.methods.harvest('0xfa86aa141e45da5183B42792d99Dede3D26Ec515', 0).call({from:'0xfa86aa141e45da5183B42792d99Dede3D26Ec515'})

&#x20;const \_minAmount = amount\*(1-0.003)

2.0xfa86aa141e45da5183B42792d99Dede3D26Ec515.methods.harvestConcentratorCompounder('aToken address'', \_minAmount)

### Harvester harvest

1\. const amount =vaultContract.methods.harvest(pid, '0xfa86aa141e45da5183B42792d99Dede3D26Ec515',0).call({from:'0xfa86aa141e45da5183B42792d99Dede3D26Ec515'})

&#x20;const \_minAmount = amount\*(1-0.003)

2.0xfa86aa141e45da5183B42792d99Dede3D26Ec515.methods.harvestConcentratorVault('vaultContractAddress address'', pid, \_minAmount)

