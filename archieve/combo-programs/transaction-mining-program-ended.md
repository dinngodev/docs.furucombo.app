# Transaction Mining Program (ended)

![](https://miro.medium.com/max/3200/1\*PqmMtUn5nyV4YyXk8Yz7Gw.png)

In our [previous article](https://medium.com/furucombo/announcing-combo-token-launch-53ea05a68e74), we talked about COMBO token’s distribution plan. We mentioned that in phase 2 of the event, we would launch a finely structured transaction mining program! Hence, in this article, we are going to share how this transaction mining program works and how to participate! The program will last for two months, starting at [3:00 AM (UTC) on Jan 15, 2021](https://savvytime.com/converter/utc-to-taiwan-taipei-ca-san-francisco-ny-new-york-city-united-kingdom-london/jan-15-2021/3am).

## **How does it work** <a href="d608" id="d608"></a>

The core value of this transaction mining program is very simple － _**you use Furucombo, you get COMBO token.**_ The main purpose of this is to distribute the COMBO tokens to our users and to COMBO holders fairly, and it’s also the first stage of our growth campaign to incentivize more users onboard. We hope it will bring significant growth and benefit to our esteemed community.

Unlike most liquidity mining programs that require participants to stake their tokens into the pool to farm yields, with our program, we focus on trading volume and staking amount but we also give rewards to those who don’t stake.

As stated in [COMBO tokenomics](https://medium.com/furucombo/introducing-combo-token-99f34eb05295) article, the future of Furucombo is in the hands of our community. Hence, upon completion of the first stage, we will let the community decide our next stage campaign to distribute the remaining COMBO tokens. Now, let’s get into the details of the transaction mining program.

## **Program details**

The transaction mining program will distribute COMBO tokens as rewards on a weekly basis. We calculate rewards based on two factors:

* Your weekly trading volume from eligible cubes (rank factor)
* The amount and length of time of your staked tokens (weight factor)

> This means,\
> _The more you trade, the more COMBO you get. The more and the longer you stake, the heavier weight you get to multiple rewards._

### **1. Eligible transactions** <a href="3b18" id="3b18"></a>

If you use Furucombo to send out a transaction that includes cubes and tokens listed below, then you’re eligible to get COMBO token rewards based on your volume. Since we want to encourage everyone to participate in this program with the lowest bar to join, we specifically design the rewards to let every eligible cube user get COMBO rewards without the need to stake any tokens. Namely, you just use Furucombo as usual to perform your strategies and you can earn free COMBO tokens at no cost.

**Eligible cubes:**

* Maker Generate/Payback/Deposit
* Aave V1 & V2 Deposit
* Compound Supply/Repay/Smart Borrow
* Uniswap V2 Swap
* 1inch Swap
* Curve Swap
* Yearn Deposit

**Ineligible tokens:**

* Tokens without Coingecko price feed would be ineligible, for example: pool token.

For Swap cubes, we calculate the weekly trading volume with “output” token, but both input and output tokens are required Coingecko price feed to make the swap cube eligible.

**Important:** Staking and transactions from smart contracts will not be counted. For example, Argent and DappLogic will not be counted as the behavior of these wallets are quite unique. Quick check? If your transaction has the tag “Interacted With (To): Furucombo: Proxy vx.x.x” on etherscan, it will be counted.

### **2. Pools** <a href="22fc" id="22fc"></a>

Pools are weight factors used to magnify your rewards. There are two pools on Furucombo where you can stake specific tokens to increase your weight.

* COMBO Pool: you stake COMBO token
* COMBO/ETH Uniswap V2 Liquidity Pool: you stake LP token

Please note that the weight is calculated based on **staking area** = **staking amount** x **staking duration**. In other words, you’d want to stake as many tokens and as longer period as you can to optimize your rewards.

### **3. Rewards Calculation** <a href="f3c0" id="f3c0"></a>

You can find the script of the rewards calculations through the link here: [https://github.com/dinngodev/furucombo-reward-scripts](https://github.com/dinngodev/furucombo-reward-scripts)\
In summary, reward distribution is decided by weekly trading rank, staking amount, and staking duration.

* Weekly trading rank: higher trading volume in a round gives higher trading rank, e.g., user A/B/C’s trading volume are 10/100/1000 USD, their trading rank are 1/2/3.
* Staking amount: the amount of token in a staking contract, e.g., user A/B/C stakes 100/50/20 COMBO in the staking contract
* Staking duration: the duration of token in a staking contract, e.g., user A/B/C’s staking duration is 46500 blocks \~= 1 week.
* Share of rewards = (trading\_rank \* staking\_amount \* staking\_duration)

Scenarios:

* User Alice: Make trades and stake tokens: high rewards
* User Ben: Make trades but no staking: some rewards
* User Charlie: No trades but stake tokens: no rewards
* User Dora: No trades and no staking: no rewards

Rewards allocation:

* Total 187,500 COMBO per week

\- COMBO Pool: 46,875 COMBO\
****- COMBO/ETH Uni LP Pool: 140,625 COMBO

![Claim COMBO](https://miro.medium.com/max/680/1\*Z-mjZ3Z8NTbdk4JTh8FFHg.png)

> What's the difference between COMBO and ETH-COMBO LP pool?\
> Answer: The competition is different.
>
> COMBO Pool: Every traded user no matter stake or not would share the rewards in this pool. If you made trades and have staked 0 COMBO, we will treat you as staked 250\* COMBO when calculating the rewards; if you made trades and have staked 1000 COMBO, we will treat you as staked 1250 COMBO when calculating the rewards. Besides, there’s a trading volume cap of $1000 USD\*. This means that users with $1000 or $1000+ weekly trading volume will share the same trading rank.
>
> COMBO/ETH Uniswap V2 Liquidity Pool: Only people who stake could share the rewards in this pool. Besides, there’s a trading volume cap of $1 million USD\*. This means that users with $1 million or $1 million+ weekly trading volume will share the same trading rank.
>
> \*The numbers are updated after [the Feb 22–24 community vote](https://discordapp.com/channels/518722025095954434/803945177780846592/814082120115945472).

## How to participate <a href="0743" id="0743"></a>

Anyone can participate in the transaction mining program. All you need to do is use Furucombo to send out transactions that include eligible cubes and tokens. To maximize rewards, we recommend that you stake COMBO token or COMBO/ETH Uni-V2 LP token as soon as you own some. Because the earlier you stake, the bigger your staking area will be, hence higher rewards.

In addition, sometimes you may want to claim COMBO tokens and then stake them right away. In this case, you must set up cubes in this order otherwise the transaction will fail:

How? → [https://go.furucombo.app/e0fQg](https://go.furucombo.app/e0fQg)

* Claim COMBO
* Add funds — COMBO
* Stake COMBO

![Claim & Stake COMBO](https://miro.medium.com/max/5760/1\*WS\_nVG67Uxc5GJo9qzCWtA.png)

The reason why you must put an “Add funds” cube in the middle is because when Furucombo executes the “claim COMBO” cube, those COMBO tokens go straight to your wallet but not Furucombo proxy. In order to let Furucombo proxy to continue executing the “Stake COMBO” cube, you need to send the just claimed COMBO back to Furucombo proxy.

That’s it! Enjoy earning COMBO tokens every week. If you have any questions on this, our team is standing by in [Discord](https://discord.furucombo.app) to answer any questions. Thanks for participating in the Furucombo community!

📮 Official COMBO Address: 0[xfFffFffF2ba8F66D4e51811C5190992176930278](https://etherscan.io/token/0xfFffFffF2ba8F66D4e51811C5190992176930278)
