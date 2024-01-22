# Contracts

{% embed url="https://github.com/AladdinDAO/deployments/blob/main/deployments.mainnet.md#fx-protocol" %}

#### f(x) protocol

* [Fx.Governance](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/deployments/mainnet/Fx.Governance.json)
* [Fx.stETH](https://github.com/AladdinDAO/aladdin-v3-contracts/blob/main/deployments/mainnet/Fx.stETH.json)

**Governance**

| Name                  |                   Address                  | Notes |
| --------------------- | :----------------------------------------: | ----- |
| TokenSale Round1      | 0x3eB6Da2d3f39BA184AEA23876026E0747Fb0E17f |       |
| TokenSale Round2      | 0x674A745ADb09c3333D655cC63e2d77ACbE6De935 |       |
| FXN                   | 0x365AccFCa291e7D3914637ABf1F7635dB165Bb09 |       |
| veFXN                 | 0xEC6B8A3F3605B083F7044C0F31f2cac0caf1d469 |       |
| TokenMinter           | 0xC8b194925D55d5dE9555AD1db74c149329F71DeF |       |
| GaugeController       | 0xe60eB8098B34eD775ac44B1ddE864e098C6d7f37 |       |
| SmartWalletWhitelist  | 0xD71B8B76015F296E53D41e8288a8a13eAfFff2ea |       |
| Vesting FXN           | 0x2290eeFEa24A6E43b26C27187742bD1FEDC10BDB |       |
| ManageableVesting FXN | 0x0E4f31a2f48418c90F5e9fa84Bf761D832C54ceD |       |
| CvxFxnVestingManager  | 0x43fCFe9F128b5e4271c7E25C47eFe91bA8896220 |       |
| SdFxnVestingManager   | 0xA2FaffE31153e5E60F2352e3ed28ff973309C156 |       |
| MultipleVestHelper    | 0x267b7A1d56d624293Ba1819f30B5bf0F12A524E4 |       |

**f(x) on stETH**

| Name                        |                   Address                  | Notes      |
| --------------------------- | :----------------------------------------: | ---------- |
| fETH                        | 0x53805A76E1f5ebbFE7115F16f9c87C2f7e633726 |            |
| xETH                        | 0xe063F04f280c60aECa68b38341C2eEcBeC703ae2 |            |
| stETHTreasury               | 0x0e5CAA5c889Bdf053c9A76395f62267E653AFbb0 |            |
| Market                      | 0xe7b9c7c9cA85340b8c06fb805f7775e3015108dB |            |
| RebalancePool               | 0xa677d95B91530d56791FbA72C01a862f1B01A49e | deprecated |
| ReservePool                 | 0x5d0Aacf75116d1645Db2B3d1Ca4b303ef0CA3752 |            |
| FxGateway                   | 0x5c28b966aB37cFB9397bBc04595f91F0fBf06d9b |            |
| stETHGateway                | 0x9bF5fFABbF97De0a47843A7Ba0A9DDB40f2e2ed5 | deprecated |
| wstETHWrapper               | 0xb09e34dD25d5E88a1E9Ff6F6418109927675B658 |            |
| StETHAndxETHWrapper         | 0xC2BdBF323304eaBd9260b42E4d0d429Ca3481d6E |            |
| FxETHTwapOracle             | 0xa84360896cE9152d1780c546305BB54125F962d9 |            |
| ChainlinkTwapOracleV3 ETH   | 0x460B3CdE57DfbA90DBed02fd83d3990a92DA1230 |            |
| ChainlinkTwapOracleV3 stETH | 0xD24AC180e6769Fd5F624e7605B93084171074A77 |            |

**Rebalance Pool (fETH)**

* RebalancePoolRegistry: 0x4eEfea49e4D876599765d5375cF7314cD14C9d38
* RebalancePoolSplitter: 0x79c5f5b0753acE25ecdBdA4c2Bc86Ab074B6c2Bb

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

| Token Burner      |                   Address                  |  Note |
| ----------------- | :----------------------------------------: | :---: |
| PlatformFeeBurner | 0x6440e21A3634C319c69CEf8d17601DBC4E97C3dB | stETH |

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
