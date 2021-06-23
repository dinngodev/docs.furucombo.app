---
description: 'Tutorial: Limit Order'
---

# Limit Order

![](https://lh4.googleusercontent.com/oZ6b3lkNl-IQ8C_8bh6rhsYVdaJTzyZmchLnzj0YCpu9tcSCzGZ8VaXOBxu_3N6V_L9_jk8PyGa40rZxgyVqDlqbuqOwwTAqowXDhuy_yD8n-2ZEXnV_i5N0Q5pxgOwvS1HGWnOB)

In general, a limit order is a type of order to purchase or sell a token at a specified price or better. For example, I want to sell ETH when the price of ETH surges to $3000 in US dollars, then I could use a limit order to do that.

Today we are thrilled to share that Furucombo supports limit order. It’s our first automation feature, and it’s powered by [Gelato Network](https://gelato.network/). This will soon be extended to include more advanced conditions, including the changes in gas fees as well as in average percentage yield \(APY\), not to mention to set a trigger with time frame. The limit order function will also be added to Furucombo’s existing drag and drop tool that allows users to set up custom DeFi combinations, or “combos’’, that are bundled together into one transaction in the near future.

In this article, we will walk you through a limit order example on Furucombo. Let’s go!

## We will cover

* How to send a limit order on Furucombo
* How to track the status for a limit order

### How to send a limit order on Furucombo

When you create a limit order on Furucombo, you create a scheduled task. And the task will be executed when the specified price matches on Uniswap.

For example, Sam wants to sell ETH when it’s price surges. She can use the limit order to create a task: pay 1 ETH to receive 3000 DAI when 1 ETH equals to 3000 DAI.

Once Sam submits the limit order, the 1 ETH will be parked on Gelato Network, waiting for the ETH price to reach 3000 DAI in Uniswap. As long as the ETH price can cover 3000 DAI plus the gas fees to execute the swap, some bots from the Gelato Network will have the incentives to execute the swap, pay the gas fees, send the 3000 DAI to your wallet, and take the left amount as its own reward.

Limit order is now live in the Explore page, go create your [limit order here](https://go.furucombo.app/mNtqI).

![A limit order to sell ETH when ETH price surges to 3000 DAI.](https://lh3.googleusercontent.com/_fLEA3aOCwq6DqHnKUnuh-B95WgGhUBeUgOAcJ1i1LRd661SNtzesslzREEJ8q6WIqP0hwSewrKIFv521so1zEKYMBZCCOK66P4wPzwwtgBEfrV9DjMnukRsJL-jPESPB-DC_y0H)

### How to track the status for a limit order <a id="0e61"></a>

Once you send out the order, you can navigate to the Automation dashboard under the wallet button, where you can see all your limit order tasks.

* Scheduled: This is the list for unexecuted limit orders. They are waiting for the target price to be reached. You can cancel a limit order and get the funds returned to your wallet by clicking the trash icon, and that would require you to pay some gas fees as well.
* Completed: This is the list for executed limit orders.
* Stopped: This is the list for cancelled limit orders.

![A limit order is to schedule a trade to be executed when the price hits.](https://lh4.googleusercontent.com/aNn1hg0zs3Dgny4RnBscZjxAp07II4tRyt8LeLRbzsbTs4XhqIsYk7vYfLlbO78Ri_ZzGdxt6bZT3jdjDRKgXJmrbR7reOA2cWtLMIhFWs-D7s9wvM9MhkH66nRUj4jc0A1Whpc3)



