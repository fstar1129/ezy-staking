# Getting Started
## To start project

In the project directory, you can run:

``` bash
npm start
```

# Smart Contracts Addresess

You can find all the smart contract address here. Currently this addressess are on BSC Testnetwork.
- EZY - 0x4757DFC0FAe90940E5F293F1F45eae1bF3EF1310
- USDT - 0x2e47c10a3d5c3c365217d37fbeaad82df218fb50
- Liquidity Pool - 0x68E9573084891f84e70c026b40E02e832564E50f
- LiquidityRouter - 0x8F51586957Dd3Fe98f93790c678aBF60A764b1B6
- Stacking - 0xaFF08cf1D2e1c4573e4e87B2257c7E8D15AAe747

To view this verified contract on testnet click on this link.
[BscTestNet](https://testnet.bscscan.com/)

## Working Flow
---
When you start your application it will open on [localhost:3000](http://localhost:3000/)

- Firstly, Connect your metamast wallet via clickong on SignIn button. After successful signin on the right network which is BSC testnet. The available balance on Add Liquidity will be updated.
- You can find the 3 input field of EZY token, USDT token and the duration of the staking. this 3 field is of to add liquidity into the pool.
- When you enter the amount for the first time you have to approve both the amount for the first time. For that you can find 2 Approve EZY and USDT button below it. This will approve the MAX amount to the Liquidity Of ERC20 Smart Contract. 
- Now, if you enter the amount in any field it will automatically calculate the another amount of the same required.
- To enter the max amount in the input you can find the MAX button on the right corner of input field.

``` diff
! Note: If there is no liquidity then respective other token amount will not calculated automatically and user should input both amount. That is the ratio of pool
```
### The plan level of the input amount

The below table will describe you about the diffrent plans and it's min and max amount range.

| Plan | Min amount | Max amount | Min Duration
| ----------- | ----------- | ----------- | ----------- 
| Plan0 | $2000 | $50,000 | 1 Month
| Plan1 | 50,000 USDT | 250,000 USDT | 3 Month
| Plan2 | 250,000 USDT | 500,000 USDT | 3 Month
| Plan3 | 500,000 USDT | 1,000,000 USDT | 3 Month
| Plan4 | 1,000,000 USDT | - | 3 Month

- For the above plan, the minimum investment amount should be $2000. And for the plan0 you will be providing both Token EZY and USDT from your account.
- From Plan1 and above, you will provide only USDT amount and if the Liquidity Router smart contract doesn't have enough EZY token you will ask to **send mail** to the owner.
- The duration is the time of how long you are willing to provide liquidity of both token.
- once the owner mint the requird amount and trnsfer it to the smart contract you can now able to provide Liquidity function on the Blockchain smart contract.

## Your Staked token
Click on the **View Staked Token** button. This will show your current staked token list and it's information.

> Here you can find 3 buttons.
1. Unstake
2. Reinvest
3. Claim Reward

The first 2 buttons will be disabled for the time priod of the End Time. Once the End time will pass then after this button will be available.

---
### Unstake Button
- This button is for unstake all the amount that you have invested.
    - For all Plan You can only unstake 100% of the amount.

### Reinvest Button

- This will increase the **End Time** of the invested amount.

### Claim Reward Button

- This button is use for claiming the reward **(In EZY token)** you got from the investment. See the 6th column for the reward.







