# Getter functions
1. isStakeholder: check if an address is a stakeholder or not
2. stakeOf: returns the amount of stake
3. rewardOf: returns the amount of reward


# Setter functions
1. depositToken: stake token
2. depositPair: stake token with NFT
3. withdrawToken: unstake token that is being staked
4. withdrawNFT: unstake NFT that is being staked
5. claimReward: withdraw reward that comes from stake
6. modifyRewardRate: change the rate of reward(only called by owner)

internal functions
_distributeReward: distribute rewards to staker

# reward rate
reward rate * (current time - start time of staking)

# file structure
Context.sol is a simple contract that gets caller's address and data

ReentrancyGuard is for preventing double call of a function

ERC20 is an interface for ERC20 token

IERC721 is an interface for ERC721 token

