# Risk Management and fxUSD Reserve

fxUSD will be backed exclusively by stable-leverage pairs using ETH LSD base tokens, and at launch those will be limited to stETH and sfrxETH. New LSDs may be onboarded to expand the fxUSD reserve at some point, but each new backing LSD will be subject to risk management review, parameter setting and community governance approvals prior to being allowed into the fxUSD reserve.

Risk management will be implemented at the protocol level by setting deposit caps for each LSD, as well as a cap on the total dollar value each LSD may contribute to backing fxUSD. This simple two-layer mechanism allows the protocol to set limits on the growth of the individual stable-leverage pair separately from limits on its inclusion in the fxUSD backing. In turn, this control enables the protocol to allow LSDs to grow their TVL in the protocol without necessarily and immediately taking the risk of that growth on in fxUSD.

Withdrawals from any rebalance pool become fxUSD.

<figure><img src="https://lh7-us.googleusercontent.com/GkhzKrvYEJDb4YBIJ_5kEhe591SnR8ft_aSLWH63lGXAkTe91vqfvQZW_hHm0MOwR5h1qBbrhCoTKDPmnxwawGo3PCW175Yh6uLpPiBFkIOEpxeZsU41U_aki9JA-VFDEdhcIcge-hbqSM1RwUem-SQ" alt=""><figcaption></figcaption></figure>

fxUSD can be returned to rebalance pools so long as it has sufficient appropriate tokens in its reserve. Once there it can be left or immediately redeemed for ETH LSDs from the reserve.

<figure><img src="https://lh7-us.googleusercontent.com/IV1SN3bY6r-wquoRFowHUXI935g10cev7G_D7Gyth8HXj0IfWITXqP4nX6PxHPG4ZahFZ5f8VCDQ1vUCfCEuRLy0H1S8mdVkqtJUDG5MbUOunbPcguv9htZG8lDbaaTfGGtt0HVL9OAbKKcnczrLp2E" alt=""><figcaption></figcaption></figure>

\
\
