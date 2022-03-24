---
description: What does liquidation mean, and how can you avoid getting rekt?
---

# What is liquidation

![](<../../.gitbook/assets/G Copy (1).png>)

Liquidation occurs when an investor cannot meet the margin requirement for their leveraged position & the underlying collateral tokens will be converted to pay for the liquidation.

### Liquidation vs Forced liquidation <a href="#1cc2" id="1cc2"></a>

**Liquidation:**\
Means selling collateral for cash, or its equivalents.

**Forced liquidation:**\
Occurs when a trader’s position is closed forcibly by lending protocols as the trader ran out of the initial margin used to open the position.

### What causes a forced liquidation? <a href="#0ce9" id="0ce9"></a>

When the price begins to move against the trader’s expectation (either long or short position), the losses are paid for from the margin provided. If the losses surpass the margin provided, the position gets liquidated.

### How to avoid getting liquidated? <a href="#966f" id="966f"></a>

1️⃣ Know the liquidation rules before you open a position.

2️⃣ Raise your collateral ratio by depositing more collateral or repaying part of your loan. It’s important to monitor your collateral ratio & keep it high enough to avoid liquidation.

3️⃣ Don’t leverage too much.\
Leveraged positions are prone to volatile price swings, which may cause a trader’s investment to plunge into a negative balance in a very short time period. Measure how much risk can you afford to take before you open a position.

### Know how to self-liquidate! <a href="#53f8" id="53f8"></a>

4️⃣ Self-liquidation means you repay the loan with the fund generated from the sale of the collateral, and you’ll get the remaining assets at the end of the trading.

### How does self-liquidation work? <a href="#0de6" id="0de6"></a>

(using Aave flashloan as an upfront fund)

a)Flashloan fund to repay all debt\
b)Withdraw all collateral\
c)Sell collateral to repay flashloan

### Let’s take a Maker position as an example. <a href="#5d52" id="5d52"></a>

Before the user self-liquidated the position, they received 0.2 DAI/USDC locked LP tokens, $441,000 debt & no cash on hand. After using the strategy, they had NO Debt & received 583 DAI.

![Self-liquidation](https://lh5.googleusercontent.com/-u22HfyWqTM8-XMJglWHEMzmdWWXzt0xd\_GNQsgpdNg\_VCtX8SqrkBDmfdq2zoYjgaW9ciewtjjMtdFEEdbd5GFuAa2GgWQN682B8u7RYwDUXwu4rhtK3UtCtyhudHErVBQvBSCi)

### too complicated? Self-liquidation tip ⤵️ <a href="#081e" id="081e"></a>

It’s pretty confusing to calculate the right amount to set up a self-liquidation combo. We got it, so we build an ultimate shortcut for you: [https://furucombo.app/explore/combo\_maker\_00001](https://furucombo.app/explore/combo\_maker\_00001)

The only thing you need to do is select a vault number that you want to close!😉

![Close Maker Vault](https://lh5.googleusercontent.com/O0h5DyRmtyue1kK3yxP4C1enL-EsyptUNfPRLlK0m1DvD75Qnr3VSouvDprvu41dT69ClY8Pd11F1hSMqlKWg5nORRGZ1uLp4i7GDslil35dW4Yl61hcJ4QLyZ9pinxQW7HrXmJI)
