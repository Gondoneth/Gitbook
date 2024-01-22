# Staking



Staking provides ALD holders with a dominant strategy that allows ALD holders to keep their share of total supply constant when no incremental bond comes into the system.&#x20;

When ALD holders stake ALD, they will receive 1:1 XALD, and get rebase rewards once per epoch.

Rebase rewards is calculated as:

&#x20;                                         $$emission_{epoch}= SupplyALD*RewardRate$$

The initial $$RewardRate=0.3\%$$

Staking yield is calculated as:

&#x20;                                        $$RewardYield=emission_{epoch}/stakedALD$$

$$stakedALD$$ is the number of ALD staked

As each epoch is 6400 blocks (1 day), staking APY is calculated as:

&#x20;                                           $$APY=(1+RewardYield)^{365}-1$$



Staking income is awarded to those who contribute to the system, with different lock-up periods. xALD enjoys compounding interest.

1. Bonded ALD goes directly into the Staking Pool and will receive xALD with a 5 day linear vesting period.
2. Staked ALD receives xALD after entering Staking Pool with a linear vesting period of 9 days.
3. Airdrop recipients automatically get xALD and enter Staking Pool with a 9 days linear vesting period. xALD can be claimed when it expires and vested xALD can be unstaked to ALD at any time.
