# Contracts

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
| VotingEscrowHelper    | 0xd766f2b87DE4b08c2239580366e49710180aba02 |       |
| VotingEscrowBoost     | 0x8Cc02c0D9592976635E98e6446ef4976567E7A81 |       |
| VotingEscrowProxy     | 0x1145f304d74f3295Fa38b82e7BB8704B0E187FA1 |       |
| TokenMinter           | 0xC8b194925D55d5dE9555AD1db74c149329F71DeF |       |
| GaugeController       | 0xe60eB8098B34eD775ac44B1ddE864e098C6d7f37 |       |
| GaugeControllerOwner  | 0x1Ca7b82c4265835C7841cf29407217D820a7DADb |       |
| SmartWalletWhitelist  | 0xD71B8B76015F296E53D41e8288a8a13eAfFff2ea |       |
| Vesting FXN           | 0x2290eeFEa24A6E43b26C27187742bD1FEDC10BDB |       |
| ManageableVesting FXN | 0x0E4f31a2f48418c90F5e9fa84Bf761D832C54ceD |       |
| CvxFxnVestingManager  | 0x43fCFe9F128b5e4271c7E25C47eFe91bA8896220 |       |
| SdFxnVestingManager   | 0xA2FaffE31153e5E60F2352e3ed28ff973309C156 |       |
| MultipleVestHelper    | 0x267b7A1d56d624293Ba1819f30B5bf0F12A524E4 |       |
| ReservePoolV2         | 0xb592E01dd77084b36430ffCB9c9D2F76fDE32631 |       |

**Price Oracle**



| Name                            |                   Address                  | Notes      |
| ------------------------------- | :----------------------------------------: | ---------- |
| ChainlinkTwapOracleV3 ETH/USD   | 0x460B3CdE57DfbA90DBed02fd83d3990a92DA1230 | 30min twap |
| ChainlinkTwapOracleV3 stETH/USD | 0xD24AC180e6769Fd5F624e7605B93084171074A77 | 30min twap |
| FxChainlinkTwapOracle BTC/USD   | 0x82012139b29BC5Ac2ff4066832c836122bC6c690 | 30min twap |
| FxChainlinkTwapOracle WBTC/BTC  | 0xe3202d6029320b6592B439bD67b7E2C154441413 | 30min twap |
| FxStETHTwapOracle               | 0xa84360896cE9152d1780c546305BB54125F962d9 | 30min twap |
| FxFrxETHTwapOracle              | 0x939c38921c961DecB3cc16f601C32d07C41cd25C | 30min twap |
| FxEETHTwapOracle                | 0x834E87262A00b0aC38eD49Cb1110838866bE4a20 | 30min twap |
| FxWBTCTwapOracle                | 0x7e94c07C6C3b2C931E9517529F56553770a7C0D2 | 30min twap |

**Liquidity Gauge**



| Name         |                 LP Address                 |                Gauge Address               |   Notes   |
| ------------ | :----------------------------------------: | :----------------------------------------: | :-------: |
| ETH+FXN      | 0xE06A65e09Ae18096B99770A809BA175FA05960e2 | 0xA5250C540914E012E22e623275E290c4dC993D11 | dual farm |
| FXN+cvxFXN   | 0x1062FD8eD633c1f080754c19317cb3912810B5e5 | 0xfEFafB9446d84A9e58a3A2f2DDDd7219E8c94FbB | dual farm |
| FXN+sdFXN    | 0x28Ca243dc0aC075dD012fCf9375C25D18A844d96 | 0x5b1D12365BEc01b8b672eE45912d1bbc86305dba | dual farm |
| crvUSD+fxUSD | 0x8ffc7b89412efd0d17edea2018f6634ea4c2fcb2 | 0xF4Bd6D66bAFEA1E0500536d52236f64c3e8a2a84 | dual farm |
| PYUSD+fxUSD  | 0xd6982da59F1D26476E259559508f4135135cf9b8 | 0xeD113B925AC3f972161Be012cdFEE33470040E6a | dual farm |
| DOLA+fxUSD   | 0x189B4e49B5cAf33565095097b4B960F14032C7D0 | 0x61F32964C39Cca4353144A6DB2F8Efdb3216b35B | dual farm |
| GRAI+fxUSD   | 0x69Cf42F15F9325986154b61A013da6E8feC82CCF | 0xfa4761512aaf899b010438a10C60D01EBdc0eFcA | dual farm |
| FRAX+fxUSD   | 0x1EE81c56e42EC34039D993d12410d437DdeA341E | 0x31b630B21065664dDd2dBa0eD3a60D8ff59501F0 | dual farm |
| GHO+fxUSD    | 0x74345504Eaea3D9408fC69Ae7EB2d14095643c5b | 0xf0A3ECed42Dbd8353569639c0eaa833857aA0A75 | dual farm |
| mkUSD+fxUSD  | 0xca554e2e2948a211d4650fe0f4e271f01f9cb5f1 | 0xDbA9a415bae1983a945ba078150CAe8b690c9229 | dual farm |
| ULTRA+fxUSD  | 0xf33ab11e5c4e55dacb13644f0c0a9d1e199a796f | 0x0d3e9A29E856CF00d670368a7ab0512cb0c29FAC | dual farm |
| fxUSD+rUSD   | 0x2116bfad62b383043230501f6a124c6ea60ccfa5 | 0x697DDb8e742047561C8e4bB69d2DDB1b8Bb42b60 | dual farm |
| alUSD+fxUSD  | 0x27cb9629ae3ee05cb266b99ca4124ec999303c9d | 0x9c7003bC16F2A1AA47451C858FEe6480B755363e | dual farm |
| eUSD+fxUSD   | 0x16b54e3aC8e3ba088333985035b869847e36E770 | 0x5801Bb8f568979C722176Df36b1a74654A9C52b5 |           |
| rgUSD+fxUSD  | 0x6fC7eA6CA8Cd2759803eb78159C931a8FF5E0557 | 0x4CA79F4FE25BCD329445CDBE7E065427ACa98380 |           |
| MIM+fxUSD    | 0xD7Bf9bb6Bd088317Effd116E2B70ea3A054cBceb | 0xDF7fbDBAE50C7931a11765FAEd9fe1A002605B55 |           |

**Rebalance Pool Gauge**



| Name    |                Gauge Address               |               Claimer Address              | Notes |
| ------- | :----------------------------------------: | :----------------------------------------: | ----- |
| fETH    | 0x9710ca7f3edd4893f399c89ea184d92cc7172e28 | 0x81243a88Dd9Fb963c643bD3f2194c2cA9CCFc428 |       |
| fstETH  | 0xf422446F7730e50B9CAb4618343425d9927b35ED | 0xCa0563ab14a87ee64d6b097B0dfC46E9B56820aD |       |
| ffrxETH | 0xB3886b8c94C8635B786b1CA88942337669BB1e1E | 0x4ae3BE52c411CC08434d28645FD391497C69c815 |       |
| feETH   | 0xf594bDfafE4197144C6459FcA611d7B868d36bEa | 0x835191186745e63f9e325E741B273ff925174d7e |       |
| fezETH  | 0xb2E43ECecA7c110c74Cf13Ba35105B0633B74E91 | 0xb259515748c75A7216a4849e67cEB166b0DAa98b |       |
| fWBTC   | 0x4E6A1dC233f264dd07b63E206Fc451d986bA9908 | 0x93670efe073e0d75BE16445779a8399E6b418004 |       |

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

**rUSD, beta = 0**



* rUSD: 0x65D72AA8DA931F047169112fcf34f52DbaAE7D18
* FxUSDRebalancer: 0x78c3aF23A4DeA2F630C130d2E42717587584BF05

**feETH & xeETH**



| Name                  |                   Address                  | Notes |
| --------------------- | :----------------------------------------: | ----- |
| Treasury              | 0x781BA968d5cc0b40EB592D5c8a9a3A4000063885 |       |
| Market                | 0x267C6A96Db7422faA60Aa7198FfEeeC4169CD65f |       |
| feETH                 | 0x9216272158F563488FfC36AFB877acA2F265C560 |       |
| xeETH                 | 0xACB3604AaDF26e6C0bb8c720420380629A328d2C |       |
| FxInitialFund         | 0x6dc7a100d09DDbF344FC4Dd0398f79500D0c2716 |       |
| RebalancePoolRegistry | 0xb1dD23468a69DFDDb7211298e609C0DB1522B2D6 |       |
| RebalancePoolSplitter | 0x015729C84A1C5E541DFbF6f0dDc59AE66527B5eD |       |
| RebalancePool.weETH   | 0xc2DeF1E39FF35367F2F2a312a793477C576fD4c3 |       |
| RebalancePool.xeETH   | 0x7EB0ed173480299e1310d55E04Ece401c2B06626 |       |
| LeveragedTokenWrapper | 0xA9414Ee8b2b2563E70174972FAa2E8B5197Feb5D |       |

**fezETH & xezETH**



| Name                  |                   Address                  | Notes |
| --------------------- | :----------------------------------------: | ----- |
| Treasury              | 0x38965311507D4E54973F81475a149c09376e241e |       |
| Market                | 0x69518D1D70AD537C41401303BDf96032338E40dE |       |
| fezETH                | 0x50B4DC15b34E31671c9cA40F9eb05D7eBd6b13f9 |       |
| xezETH                | 0x2e5A5AF7eE900D34BCFB70C47023bf1d6bE35CF5 |       |
| FxInitialFund         | 0x7612bCAbd3D66c71fF740472e063be6a74f126D1 |       |
| RebalancePoolRegistry | 0x5e3ca2A5736fb093328e4CA19A9A1966025f3905 |       |
| RebalancePoolSplitter | 0x2755EEbf220BFD31B83Fd9244B6D061bCa225311 |       |
| RebalancePool.ezETH   | 0xf58c499417e36714e99803Cb135f507a95ae7169 |       |
| RebalancePool.xezETH  | 0xBa947cba270D30967369Bf1f73884Be2533d7bDB |       |
| LeveragedTokenWrapper | 0xBeb4289491EBFE8452CfAc8830a6285E42A4742b |       |

**btcUSD, beta = 0**



* btcUSD: 0x9D11ab23d33aD026C466CE3c124928fDb69Ba20E
* FxUSDRebalancer: 0x78c3aF23A4DeA2F630C130d2E42717587584BF05

**fWBTC & xWBTC**



| Name                  |                   Address                  | Notes |
| --------------------- | :----------------------------------------: | ----- |
| Treasury              | 0x63Fe55B3fe3f74B42840788cFbe6229869590f83 |       |
| Market                | 0x56B85438F1E16a91eAc5Fe2DAAb2C3Dd57690175 |       |
| fWBTC                 | 0x576b4779727F5998577bb4e25bf726abE742b9F7 |       |
| xWBTC                 | 0x9f23562ec47249761222EF7Ac02b327a8C45Ba7D |       |
| FxInitialFund         | 0x29eE4B752fE14B0BC1F279DCA98415f2Fa6F3A8d |       |
| RebalancePoolRegistry | 0x163283D59FE2A579f2920A7F8eA19F7799B32fA0 |       |
| RebalancePoolSplitter | 0x054fAC7aA44F85A59FD41c33006336EC8b03E916 |       |
| RebalancePool.WBTC    | 0xf291EC9C2F87A41386fd94eC4BCdC3270eD04482 |       |
| RebalancePool.xWBTC   | 0xBB549046497364A1E26F94f7e93685Dc29FAd8c0 |       |
| LeveragedTokenWrapper | 0x1A17Ccf198E03858227c27205f15a4b388235DB7 |       |

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

**Rebalance Pool**



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
