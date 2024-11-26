# FAQ

**What is F(x) Protocol 2.0?**

f(x) Protocol 2.0 improves on version 1.0 by keeping the stablecoin fxUSD and enhancing the xPOSITION tool for leveraged trading. It removes liquidation risks and funding fees, offering a fully decentralized trading tool with up to 10X fixed leverage. The updated system also makes the user experience smoother and strengthens the protocol's stability, advancing the growth of decentralized finance (DeFi).

**What is xPOSITION?**

xPOSITION, a non-fungible, high-beta leveraged long position. The leveraged long position offers a powerful decentralized tool for on-chain high-leverage trading. When a user opens an xPOSITION, the process will be seamlessly facilitated by leveraging a flash loan. **This occurs through an atomic transaction**, ensuring that all steps are completed successfully or the entire transaction is reverted, maintaining the integrity of both the user’s funds and the system.

**What is the f(x) Invariant?**

The NAV of fxUSD and xPOSITION fluctuates with the price of TOKEN, ensuring that the total value of all fxUSD combined with the total value of all xPOSITIONs always equals the total value of the TOKEN reserve.

**What is Rebalance?**

When the leverage of an xPOSITION reaches a predefined threshold, the protocol automatically triggers a Rebalance operation to return the leverage back to the rebalance line. This operation involves redeeming a portion of the fxUSD to adjust the leverage back to the rebalance line. During Rebalance or Liquidation Operations, fxUSD is first redeemed from the Stability Pool and the underlying TOKEN is swapped for USDC.

**What is a Stability Pool?**

The Stability Pool is a key component of f(x) Protocol, designed to provide both stability and yield opportunities for participants. Users can deposit fxUSD and/or USDC into the Stability Pool to earn TOKEN yield and perpetual trading commissions during normal market conditions. The Stability Pool also functions as a peg stabilizer for the fxUSD/USDC AMM pool. USDC held in the Stability Pool will be exchanged for fxUSD from the AMM when favorable exchange conditions arise, allowing USDC to be swapped for a greater amount of fxUSD. Conversely, fxUSD will be swapped for USDC when it can secure a higher amount of USDC from the AMM. This mechanism ensures efficient balancing and maintains fxUSD’s peg. USDC deposits into the Stability Pool are conducted at the Chainlink oracle price to ensure accurate valuations.&#x20;

**Where did the Leverage come from?**

1. The user opens xPOSITION and sets Leverage;
2. Check the system's fxUSD minting availability;
3. Position opened, enough fxUSD is minted, or deny the transaction;
4. Rebalance occurs within a predefined threshold to maintain system stability(Redeeming/Minting of fxUSD if needed).

**Does fxUSD work on F(x) 1.0 and F(x) 2.0?**

Yes, but with some different revenue-generating mechanisms.

