# RG Staking

Purchase assets by depositing tokens and earn rewards based on your holdings. Visit [rg-staking.on.fleek.co](https://rg-staking.on.fleek.co)

## Smart Contract

The smart contract offers the following:

### Token Creation and Asset Ownership

- Users can deposit multiples of 10 tokens to purchase assets. To simplify this process, users can directly buy assets, where 1 asset equals 10 tokens. This ensures that users always deposit a multiple of 10 tokens.

### Asset Creation and Reward Distribution

- For every 10 tokens (1 asset) purchased, an "Asset" is created and associated with the user's wallet address. For instance, if a user deposits 40 tokens, they become the owner of 4 assets.

- Every 24 hours, asset owners are entitled to a reward of 0.1 tokens per asset they hold. This reward is calculated based on the number of assets owned by the user.

### Reward Pool

- A reward pool with 10,000 native tokens has been initialized to facilitate rewards distribution. The pool will be used to pay out rewards to asset owners.

### Claiming Rewards

- Asset owners can claim their earned rewards at any time during a given time frame. However, the claimable reward amount is capped at the maximum available balance in the reward pool. This ensures that the reward distribution does not exceed the available rewards.

## Reasoning around the Implementation

The implementation introduces the concept of asset ownership, where users directly purchase assets instead of depositing multiples of 10 tokens. This approach simplifies the user experience while achieving the same result.

The reward distribution follows a fair model where users are entitled to 0.1 tokens per asset they hold, and the reward pool ensures sufficient rewards for everyone.

To calculate rewards, we consider the number of assets owned by each user and the last time they interacted with the contract (bought assets, redeemed assets, or claimed rewards). This allows us to provide accurate and up-to-date reward amounts when users perform actions on the contract.

To get started, the reward pool must be initialized by sending exactly 10,000 tokens to the contract. Once initialized, users can begin purchasing assets, redeeming assets, and claiming rewards.

## Contract Links

[RGT Token]([URL](https://testnet.snowtrace.io/address/0x16855ba2Dba2485075a8C7e780d400B6c75BbC2F#code))
[RG Staking]([URL](https://testnet.snowtrace.io/address/0x4B4d54AA4a93a45f76B4608886b2f7BF5CD8cB33#code))

Happy Staking!
