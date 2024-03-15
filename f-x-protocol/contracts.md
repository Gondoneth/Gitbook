# Contracts

#### [f(x) protocol](https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#fx-protocol)

* [Fx.Governance](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/deployments/mainnet/Fx.Governance.json)
* [Fx.stETH](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/deployments/mainnet/Fx.stETH.json)

**Governance**

<table><thead><tr><th width="228.66666666666666">Name</th><th align="center">Address</th><th>Notes</th></tr></thead><tbody><tr><td>TokenSale Round1</td><td align="center">0x3eB6Da2d3f39BA184AEA23876026E0747Fb0E17f</td><td></td></tr><tr><td>TokenSale Round2</td><td align="center">0x674A745ADb09c3333D655cC63e2d77ACbE6De935</td><td></td></tr><tr><td>FXN</td><td align="center">0x365AccFCa291e7D3914637ABf1F7635dB165Bb09</td><td></td></tr><tr><td>veFXN</td><td align="center">0xEC6B8A3F3605B083F7044C0F31f2cac0caf1d469</td><td></td></tr><tr><td>TokenMinter</td><td align="center">0xC8b194925D55d5dE9555AD1db74c149329F71DeF</td><td></td></tr><tr><td>GaugeController</td><td align="center">0xe60eB8098B34eD775ac44B1ddE864e098C6d7f37</td><td></td></tr><tr><td>SmartWalletWhitelist</td><td align="center">0xD71B8B76015F296E53D41e8288a8a13eAfFff2ea</td><td></td></tr><tr><td>Vesting FXN</td><td align="center">0x2290eeFEa24A6E43b26C27187742bD1FEDC10BDB</td><td></td></tr><tr><td>ManageableVesting FXN</td><td align="center">0x0E4f31a2f48418c90F5e9fa84Bf761D832C54ceD</td><td></td></tr><tr><td>CvxFxnVestingManager</td><td align="center">0x43fCFe9F128b5e4271c7E25C47eFe91bA8896220</td><td></td></tr><tr><td>SdFxnVestingManager</td><td align="center">0xA2FaffE31153e5E60F2352e3ed28ff973309C156</td><td></td></tr><tr><td>MultipleVestHelper</td><td align="center">0x267b7A1d56d624293Ba1819f30B5bf0F12A524E4</td><td></td></tr><tr><td>ReservePoolV2</td><td align="center">0xb592E01dd77084b36430ffCB9c9D2F76fDE32631</td><td></td></tr></tbody></table>

**Price Oracle**

| Name                        |                   Address                  | Notes      |
| --------------------------- | :----------------------------------------: | ---------- |
| ChainlinkTwapOracleV3 ETH   | 0x460B3CdE57DfbA90DBed02fd83d3990a92DA1230 | 30min twap |
| ChainlinkTwapOracleV3 stETH | 0xD24AC180e6769Fd5F624e7605B93084171074A77 | 30min twap |
| FxStETHTwapOracle           | 0xa84360896cE9152d1780c546305BB54125F962d9 | 30min twap |
| FxFrxETHTwapOracle          | 0x939c38921c961DecB3cc16f601C32d07C41cd25C | 30min twap |

**Liquidity Gauge**

| Name       |                 LP Address                 |                Gauge Address               |   Notes   |
| ---------- | :----------------------------------------: | :----------------------------------------: | :-------: |
| ETH+FXN    | 0xE06A65e09Ae18096B99770A809BA175FA05960e2 | 0xA5250C540914E012E22e623275E290c4dC993D11 | dual farm |
| FXN+cvxFXN | 0x1062FD8eD633c1f080754c19317cb3912810B5e5 | 0xfEFafB9446d84A9e58a3A2f2DDDd7219E8c94FbB | dual farm |
| FXN+sdFXN  | 0x28Ca243dc0aC075dD012fCf9375C25D18A844d96 | 0x5b1D12365BEc01b8b672eE45912d1bbc86305dba | dual farm |

**Stability Pool Gauge**

| Name    |                Gauge Address               |               Claimer Address              | Notes |
| ------- | :----------------------------------------: | :----------------------------------------: | ----- |
| fETH    | 0x9710ca7f3edd4893f399c89ea184d92cc7172e28 | 0x81243a88Dd9Fb963c643bD3f2194c2cA9CCFc428 |       |
| fstETH  | 0xf422446F7730e50B9CAb4618343425d9927b35ED | 0xCa0563ab14a87ee64d6b097B0dfC46E9B56820aD |       |
| ffrxETH | 0xB3886b8c94C8635B786b1CA88942337669BB1e1E | 0x4ae3BE52c411CC08434d28645FD391497C69c815 |       |

**fxUSD, beta = 0**

* FxUSD: 0x085780639CC2cACd35E474e71f4d000e2405d8f6
* FxUSDRebalancer: 0x78c3aF23A4DeA2F630C130d2E42717587584BF05

**fstETH & xstETH**

| Name                  |                   Address                  | Notes |
| --------------------- | :----------------------------------------: | ----- |
| Treasury              | 0xED803540037B0ae069c93420F89Cd653B6e3Df1f |       |
| Market                | 0xAD9A0E7C08bc9F747dF97a3E7E7f620632CB6155 |       |
| fstETH                | 0xD6B8162e2fb9F3EFf09bb8598ca0C8958E33A23D |       |
| xstETH                | 0x5a097b014C547718e79030a077A91Ae37679EfF5 |       |
| WstETHRateProvider    | 0x81A777c4aB65229d1Bf64DaE4c831bDf628Ccc7f |       |
| FxInitialFund         | 0xe6b953BB4c4B8eEd78b40B81e457ee4BDA461D55 |       |
| RebalancePoolRegistry | 0x86e987a89Fd7345457d97b9e82906f346D61Df39 |       |
| RebalancePoolSplitter | 0x78Ef19714c8b3c71997970C156f59605A99C3ff3 |       |
| RebalancePool.wstETH  | 0x9aD382b028e03977D446635Ba6b8492040F829b7 |       |
| RebalancePool.xstETH  | 0x0417CE2934899d7130229CDa39Db456Ff2332685 |       |
| LeveragedTokenWrapper | 0x6AF422087aBF42819F764FF8DE95269036b9A8F9 |       |

**ffrxETH & xfrxETH**

| Name                        |                   Address                  | Notes |
| --------------------------- | :----------------------------------------: | ----- |
| Treasury                    | 0xcfEEfF214b256063110d3236ea12Db49d2dF2359 |       |
| Market                      | 0x714B853b3bA73E439c652CfE79660F329E6ebB42 |       |
| ffrxETH                     | 0xa87F04c9743Fd1933F82bdDec9692e9D97673769 |       |
| xfrxETH                     | 0x2bb0C32101456F5960d4e994Bac183Fe0dc6C82c |       |
| ERC4626RateProvider sfrxETH | 0x7ceD6167b5A08111dC8d0D2f9F7E482c4Da62506 |       |
| FxInitialFund               | 0xFC3862c33b54E0BBA61d966Ff51973C20be4fC62 |       |
| RebalancePoolRegistry       | 0x345a345DAd48c3504113539ce83c0cB765627B54 |       |
| RebalancePoolSplitter       | 0xb26cA48fe4Ee94a4Fe8815F7E54E99124f997540 |       |
| RebalancePool.sfrxETH       | 0xb925F8CAA6BE0BFCd1A7383168D1c932D185A748 |       |
| RebalancePool.xfrxETH       | 0x4a2ab45D27428901E826db4a52Dae00594b68022 |       |
| LeveragedTokenWrapper       | 0x823BaF74524b707d649A2a78E66DF106f5A131aB |       |

**f(x) on stETH, beta = 0.1**

| Name                |                   Address                  | Notes      |
| ------------------- | :----------------------------------------: | ---------- |
| fETH                | 0x53805A76E1f5ebbFE7115F16f9c87C2f7e633726 |            |
| xETH                | 0xe063F04f280c60aECa68b38341C2eEcBeC703ae2 |            |
| stETHTreasury       | 0x0e5CAA5c889Bdf053c9A76395f62267E653AFbb0 |            |
| Market              | 0xe7b9c7c9cA85340b8c06fb805f7775e3015108dB |            |
| ReservePool         | 0x5d0Aacf75116d1645Db2B3d1Ca4b303ef0CA3752 | deprecated |
| FxGateway           | 0x5c28b966aB37cFB9397bBc04595f91F0fBf06d9b | deprecated |
| stETHGateway        | 0x9bF5fFABbF97De0a47843A7Ba0A9DDB40f2e2ed5 | deprecated |
| wstETHWrapper       | 0xb09e34dD25d5E88a1E9Ff6F6418109927675B658 |            |
| StETHAndxETHWrapper | 0xC2BdBF323304eaBd9260b42E4d0d429Ca3481d6E |            |

**Stability Pool**

* RebalancePoolRegistry: 0x4eEfea49e4D876599765d5375cF7314cD14C9d38
* RebalancePoolSplitter: 0x79c5f5b0753acE25ecdBdA4c2Bc86Ab074B6c2Bb
* Gauge: 0x9710ca7f3edd4893f399c89ea184d92cc7172e28
* RebalancePoolGaugeClaimer: 0x81243a88Dd9Fb963c643bD3f2194c2cA9CCFc428

| Name                          |                   Address                  |                 liquidator                 | Notes      |
| ----------------------------- | :----------------------------------------: | :----------------------------------------: | ---------- |
| RebalancePool.wstETH          | 0xa677d95B91530d56791FbA72C01a862f1B01A49e | 0x17f21f468d77E6e35702a9Ae7a9da50Db7F6a4f4 | deprecated |
| BoostableRebalancePool.wstETH | 0xc6dEe5913e010895F3702bc43a40d661B13a40BD | 0x74E9234A6e03c382A01Bb942B1aF05B639371309 |            |
| BoostableRebalancePool.xETH   | 0xB87A8332dFb1C76Bb22477dCfEdDeB69865cA9f9 | 0x5a161B94c737326cA115eC46f4Eaf4eEC5037dBE |            |

**Revenue Sharing**

| Name                  |                   Address                  | Notes      |
| --------------------- | :----------------------------------------: | ---------- |
| PlatformFeeSpliter    | 0x0084C2e1B1823564e597Ff4848a88D61ac63D703 |            |
| FeeDistributor stETH  | 0x851AAEA3A2757D457E1Ce88C3808C1690213e432 | deprecated |
| FeeDistributor wstETH | 0xd116513EEa4Efe3908212AfBAeFC76cb29245681 |            |

| Token Burner      |                   Address                  |  Note  |
| ----------------- | :----------------------------------------: | :----: |
| PlatformFeeBurner | 0x6440e21A3634C319c69CEf8d17601DBC4E97C3dB | wstETH |

**Bridging**

**fETH**

* Ethereum ProxyOFT: 0xc608Dfb90A430Df79a8a1eDBC8be7f1A0Eb4E763

| Chain      | Token Address                              |
| ---------- | ------------------------------------------ |
| Ethereum   | 0x53805A76E1f5ebbFE7115F16f9c87C2f7e633726 |
| Arbitrum   | 0xc608Dfb90A430Df79a8a1eDBC8be7f1A0Eb4E763 |
| BSC        | 0xF9E10DAA647E540BF3d1334377a88361aB980e94 |
| Optimistic | 0xc608Dfb90A430Df79a8a1eDBC8be7f1A0Eb4E763 |
| Polygon    | 0xc608Dfb90A430Df79a8a1eDBC8be7f1A0Eb4E763 |

**xETH**

* Ethereum ProxyOFT: 0x535f7Ca9637A5099DB568b79a3624CFd6B5fc833

| Chain      | Token Address                              |
| ---------- | ------------------------------------------ |
| Ethereum   | 0xe063F04f280c60aECa68b38341C2eEcBeC703ae2 |
| Arbitrum   | 0x55380fe7A1910dFf29A47B622057ab4139DA42C5 |
| BSC        | 0x62C6867e4f2e63302B15cbf9b8540214a13beeac |
| Optimistic | 0xa7580d4AdC6D302D2D4C7C3dB93E9aE3F82C4617 |
| Polygon    | 0xa7580d4AdC6D302D2D4C7C3dB93E9aE3F82C4617 |

**FXN**

* Ethereum ProxyOFT: 0x808130d89fC067a7a8D9dDF4ca2abf6EB5Ed3B32

| Chain      | Token Address                              |
| ---------- | ------------------------------------------ |
| Ethereum   | 0x365AccFCa291e7D3914637ABf1F7635dB165Bb09 |
| Arbitrum   | 0x179F38f78346F5942E95C5C59CB1da7F55Cf7CAd |
| BSC        | 0xa64f68c089B3E69d48F6047d3Be513349E74b3De |
| Optimistic | 0xC752C6DaA143e1a0ba3E7Df06f3117182432b991 |
| Polygon    | 0xC752C6DaA143e1a0ba3E7Df06f3117182432b991 |
