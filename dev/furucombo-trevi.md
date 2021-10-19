---
description: 'Trevi Tutorial: Creating Your Own Reward Distribution Contract'
---

# Furucombo Trevi

![Furucombo Trevi](https://miro.medium.com/max/1400/1\*i6gTcf\_sg77m-KGcarlMPw.png)

Furucombo has developed a permissionless staking and reward distribution system which we call Trevi. It was developed as we found that most of the existing solutions (like MasterChef, Mintr) didn’t support everything we wanted to provide in a reward distribution contract.

Trevi is [open source](https://github.com/dinngodev/trevi) and [audited by HashCloak, Chainsulting, and PeckShield](https://github.com/dinngodev/trevi/tree/master/audit). We want to share to everyone in the ecosystem so every other project team can save time and money on developing their staking and reward contract.

With Trevi, you can:

* Reward more than 2 kinds of tokens for your users — no limitation!
* Add new rewards anytime.
* Add a flash loan use case for the staking position.
* Easily integrate with Furucombo.

## Terminology <a href="583f" id="583f"></a>

Before you continue reading, there are some basic terminology for your reference:

* **Trevi:** The name of the whole system. We named it after the famous fountain in Italy, Fontana di Trevi, where travelers throw coins into the fountain for good luck and romance.
* **Archangel:** This contract records the relationship between the Fountain and Angel, and manages the configuration of the flash loan-related functions.
* **Angel:** The name of the reward distribution contract where a Rewarder grants the rewards as lovely angels. One Angel consists of one type of reward. You can create several Angels if you want to provide several types of tokens as reward.
* **Fountain:** The name of the staking contract where users stake tokens in order to get rewards from Angels.

## What is Trevi? <a href="71ec" id="71ec"></a>

Trevi is an ERC20-based staking and reward distribution system. It enables project teams to manage and schedule reward distribution with ease.

The contract named Archangel manages the whole Trevi system (you can check its functions on [GitHub](https://github.com/dinngodev/trevi)). When we deploy the Archangel contract, another two contracts are generated as well — the Fountain Factory and the Angel Factory.

* With the Fountain Factory contract, anyone can create a Fountain with the contract interface to allow token staking.
* With the Angel Factory contract, anyone can create an Angel to run their rewarding program with tokens.

Important notice: **AVOID USING TOKENS THAT HAVE FLOATING AMOUNTS** (including inflationary/deflationary tokens, interest tokens or rebase tokens), which might lead to error according to the contract design policy.

Once you create the Angel(s), you are now the ‘Rewarder,’ and you can manage the reward schedule and assign which Fountain can get your reward. On the other hand, your users can stake their tokens to the Fountain you assign to earn the reward from your Angel(s).

![Furucombo Trevi schematic diagram](https://miro.medium.com/max/1260/1\*mdRyVyXQ7lNewH2x\_cqYzA.png)

## How to grant rewards through Trevi (For Rewarders) <a href="5498" id="5498"></a>

As Rewarders who plan to have a reward system, they don’t need to build any contract to start the program. They can launch the program through Trevi directly on Polygonscan.

There are only three steps to issue the rewards:

1. Create an Angel contract to store your reward
2. Assign which token staking you want to incentivize
3. Set reward distribution rate and schedule

### 1. Create an Angel contract to store your reward <a href="70fd" id="70fd"></a>

First, a Rewarder needs to create the Angel contract through the [Angel Factory contract](https://polygonscan.com/address/0x66Ab9f76e7822B7160E22f8b02Dbd2D757FabF32#code) interface. You can call the function **`create(address reward)`**_** **_of the Angel Factory to create the Angel. The parameter **`reward`** is the token address of the reward you provide.

![Angel Factory Contract](https://miro.medium.com/max/1260/0\*vas5yjUIyYgWRcv6)

### 2. Assign which token staking you want to incentivize <a href="e655" id="e655"></a>

Secondly, decide which Fountain(s) you want to incentivize. A Rewarder can call the function **`add(uint256 allocPoint, address _lpToken, address _Rewarder)`** to assign the Fountain(s) to receive the reward in the [Angel](https://polygonscan.com/address/0x062ffe63b7a0d7f27a8105e717c6ea45e5848ad3#code)(s).

* You can reward many staking pools at the same time, thus you can assign different distribution weights among Fountains with the **`allocPoint`** parameter.
* **`_lpToken`** is the token address that you want to incentivize.
* **`_Rewarder`** is the contract customized developed by the Rewarder. If the Rewarder wants to do some specific behavior based on the staking system, the Rewarder can assign the contract address to **`_Rewarder`**.

![Angel Contract](https://miro.medium.com/max/1260/0\*wFDkSXZXh17x64JU)

Note: You may need to create a Fountain beforehand if the token you want to incentivize or to stake does not exist in the Trevi system yet. You can call the function **`create(ERC20 token)`** of the [Fountain Factory](https://polygonscan.com/address/0xDE7DBC03c90b0C6029F435865Cd92212D0e0cAc3#code) to create the Fountain(s).

![Fountain Factory Contract](https://miro.medium.com/max/1260/0\*z6rk2ip\_ajXINEmB)

### 3. Set reward distribution rate and schedule <a href="633c" id="633c"></a>

Now the Rewarder is ready to kick-off the reward distribution. There are two ways to set the distribution rate and schedule.

* **`addGraceReward(uint256 _amount, uint256 _endTime)`**
* **`setGracePerSecond(uint256 _gracePerSecond, uint256 _endTime)`**

Both of the approaches will transfer the reward tokens from the caller address to the Angel contract. Please make sure you approve an adequate amount to the Angel contract before calling the function.

**`3-A. addGraceReward(uint256 _amount, uint256 _endTime)`**

Rewarders need to assign the total rewarding token amount and the end time of distribution. The Angel contract will calculate the distribution rate based on the provided amount and end time.

![Angel Contract](https://miro.medium.com/max/1260/0\*FEHiXRcodj0pLVLY)

**`3-B. setGracePerSecond(uint256 _gracePerSecond, uint256 _endTime)`**

Rewarders provide the distribution rate and the end time of the distribution. The Angel contract will calculate how many reward tokens will be allocated based on the provided distribution rate and end time.

![Angel Contract](https://miro.medium.com/max/1260/0\*ISzVFXC17bSnL2NB)

That’s it! After the above 3 steps, the reward program will start to run. It will distribute the rewards to the user who stakes tokens to the Fountain every block based on the configuration you set up.

## How to earn rewards from Trevi (For Stakers) <a href="20c7" id="20c7"></a>

As a user who stakes tokens to earn rewards, it is easy to earn multiple rewards with Trevi. Users only stake their tokens to a single staking contract, and they could get the rewards from different Angles. How to do it exactly? There are three steps:

1. Deposit the staking token to a Fountain
2. Sign up for the available rewards from Angels
3. Accumulate and claim the rewards over blocks

### 1. Deposit the staking token to a Fountain <a href="bf9c" id="bf9c"></a>

Users need to stake their tokens to the Fountain. Every token address will have a unique Fountain contract, and users can call the function **`deposit(uint256 amount)`** of that Fountain contract to stake the specific token.

The deposit function will transfer the tokens from the user’s address to the Fountain contract. Thus please make sure the user approves an adequate amount to the Fountain contract before calling the function. Once the deposit transaction goes through, the user will receive FTN tokens from the Fountain, representing the tokens the user deposits to Fountain.

![Fountain Contract](https://miro.medium.com/max/1260/0\*A3ZBwf\_DgCeFzhkI)

### 2. Sign up for the available rewards from Angels <a href="de50" id="de50"></a>

Before starting to earn the reward, there is one more thing the users need to do. Users need to select which available rewards they want to have. Sign up for more types of rewards mean that users have a chance to earn more rewards, but it would cost more gas when users do any other operation (e.g., unstake token, transfer FTN token, etc.). Users can call the function **`joinAngel(address angel)`** of the Fountain to sign up for a single type of reward, or the function **`joinAngels(address[] angels)`** of the Fountain to join multiple types of rewards from multiple Angels.

Once the transaction goes through, the Angels will start to calculate the rewards based on the staking balances on the Fountain.

![Fountain Contract](https://miro.medium.com/max/1260/0\*b0yt\_N9xcDAYZlb1)

### 3. Accumulate and claim the rewards over blocks <a href="85e9" id="85e9"></a>

The reward is distributed every block, and users can decide when to claim the accumulated rewards. Users can call the function **`harvestAll()`** of the Fountain to claim all available rewards. Alternatively, they can call the function **`harvest(address angel)`** of the Fountain to claim the reward from the specific Angel contract.

![Fountain](https://miro.medium.com/max/1260/0\*Iz8Eoc-9eiux8H6l)

Note: The reward is accumulated per address, it means that once you transfer a FTN token to another address, the accumulated rewards will still be claimable only by your original address, and the new address will need to sign up for the available rewards to start to accumulate its claimable reward.

## Last but not least <a href="f5b3" id="f5b3"></a>

We have covered the basic functions of Trevi in this tutorial, while there are many other special features in Trevi such as: flash loans of Fountains and Angels, harvest permits, and join permits. If you are interested in more about Trevi, visit the repository on our [GitHub](https://github.com/dinngodev/trevi) to find out more details. For more information such as contract addresses, you can refer to our [Gitbook](https://docs.furucombo.app). Whether you are a Rewarder, user, or developer, we welcome everyone to use our Trevi reward distribution contract to build your project.
