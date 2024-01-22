# The Furnace

### <mark style="color:blue;">What’s the deal with the Furnace?</mark>

When real tokens enter the system from a yield/bribe harvest, synthetic clevTokens are minted against them 1:1. Those clevTokens are distributed to the depositors (if they have debt, it is paid down), while the real harvested tokens are deposited in the furnace over a short vesting period (1-2 weeks) where they are available for swapping. Once in the Furnace, these tokens are swapped for their clevToken equivalent at par (1:1), then the clevTokens are burned.

### <mark style="color:blue;">How can I use the Furnace to earn CVX, FRAX, etc.?</mark>

Harvested Tokens like CVX (or FRAX, CRV, etc. eventually) enter the Furnace linearly over a 1-2 week period after each harvest. If there are clevTokens deposited in the furnace waiting to be swapped, each depositor is allocated a share of the real Tokens proportional to their share of the total clevTokens deposited.

You can buy clevTokens at a discount on Curve, then exchange them over time for their real equivalents in the Furnace.

### <mark style="color:blue;">What is rebonding?</mark>

Rebonding is when you claim your available Tokens from the furnace, then swap them for even more clevTokens (the discount shows how much extra you will get on Curve) and then deposit those clevTokens back in the furnace, so that you receive a bigger share of the ongoing harvest.

### <mark style="color:blue;">What is the daily burn rate?</mark>&#x20;

As real Tokens are emitted to the Furnace, they are swapped for their clevToken equivalent which are burned. If you deposit clevTokens to the Furnace, the burn rate % shows approximately the fraction of those that will be converted to real Tokens each day after.

### <mark style="color:blue;">What are “CVX/Tokens to be allocated”?</mark>

Each time a harvest occurs, new Tokens are emitted into the Furnace over a period of 1-2 weeks, where they are swapped for clevTokens. The “Tokens to be allocated” stat indicates how many real Tokens from the previous harvest remain to be allocated in the Furnace over the rest of the current epoch. Each harvest replenishes the tokens to be allocated.
