# Other FAQ

## 🧠 Arbitrage strategies

### What is arbitrage?

In many ways, crypto arbitrage is just like fiat or sports arbitrage. The main idea here is simple: you try to benefit from price differences for the same asset on different markets or exchanges.&#x20;

Investopedia describes arbitrage as “the simultaneous purchase and sale of an asset to profit from an imbalance in the price. It is a trade that profits by exploiting the price differences of identical or similar financial instruments on different markets or in different forms.”

In other words, **buy low and sell high**!&#x20;

Related reads:&#x20;

* [Arbitrage in DeFi by The Block](https://www.theblockcrypto.com/post/45750/exploring-defi-trading-strategies-arbitrage-in-defi)

### What does a profitable combo look like?

![](../../.gitbook/assets/profitable.png)

* There is **no** initial funds

{% hint style="danger" %}
If you see initial funds section appears, that means this is not a profitable combo. The worst case is that you lose the initial funds and get nothing back.&#x20;
{% endhint %}

* You will receive
  * Assets shown in this section are profits from the combo.

### How to make a profitable combo?

* First and foremost, you need to find an arbitrage opportunity.&#x20;
* Taking gas costs into consideration, arbitrage combos cost more than average combos due to the complexity of the actions. This is a primary cost factor influencing the profitability of the trade.
* Remember there are many bots front-running trades at all times. So there's a chance that your combo may be front-ran by bots.
* Arbitrage combos have a higher chance to fail as the combo setup usually has a high dependency on each cubes' outputs. That being said, once the opportunity vanishes, your combo fails and you lose the gas fee you just pay.&#x20;

## 👛 Wallet

### I don't see Coinbase wallet in the menu

If you don't see Coinbase Wallet, click Wallet Connect and scan the QR code with your Coinbase Wallet app.

### Can I use MetaMask on Brave?

Follow [this tutorial](https://www.loom.com/share/bee83b1e0d724779aa4d22c9d8a242c0) to let Furucombo connect your MetaMask on Brave.

The reason behind this is because Brave just update their setting on how to connect "Web3 provider for using Dapps".\
​\
We will keep investigating this issue and make sure it is up to date.

### I can not connect to the platform

* Make sure to select the correct network (Ethereum Mainnet), normally on the wallet provider you can switch the network on the settings options.
* On Ledger natively or over Metamask:
  * Make sure to unlock and select Ethereum app.
  * Make sure Contract data is allowed on the Ethereum app settings.
* Coinbase
  * Use the scan QR code to connect.
* Wallet connect
  * Use the scan QR code to connect
* Fortmatic
  * Make sure to switch to Ethereum Mainnet.

## ⛽️ Gas

### Why is the gas fee so high?

It depends on how many cubes you use and how busy the Ethereum network is. You can click “Send” button to estimate the gas cost. Your wallet (e.g. MetaMask) will pop up and tell you how much you may spend on the gas fee.

### Can I know how much gas before send?

Unfortunately, you are not able to get the estimate of gas before hitting the send button.

### How can I set up the gas price?

You can adjust gas price and gas limit when using MetaMask wallet. Upon hitting the send button, you'll see a MetaMask pop-up. Click "EDIT" then you will see choices of speed.&#x20;

To customize the transaction fee, select Advanced Options:

You can manually enter Gas Price (GWEI) and Gas Limit.  You can also click on the Live Gas Predictions graph.

![](<../../.gitbook/assets/image (9).png>)

### Should I reduce gas limit?

No, you shouldn't. The gas limit is the budget of the transaction. The unused gas will be refunded to your wallet. However, if the gas costs more than your gas limit, everything will be reverted but the gas will NOT be returned.

## 📖 Other FAQs

### How do I adjust initial funds?

The amount of initial funds is auto-updated.

You just need to adjust the numbers in the cubes, then the required amount of initial fund would be updated accordingly.

### Why do I need to sign two times?

Normally you need to send 2 transactions to process a non-ETH token transfer.\
For example, If you want to swap DAI to COMP, you have to sign twice on your wallet:

1. Approve: to grant Furucombo the permission to move your tokens.
2. Send: to execute your transaction. In this example, to swap your DAI to COMP.

### How many times do I have to approve?

It depends on what tokens you have and what cubes you are going to use.

The number of times you need to approve is based on how many conditions below are met, and how much the amount of approved ERC-20 tokens that you grant Furucombo to move.

* First time to use ERC20 tokens as initial funds
* First time to use any of the below cubes:
  * Maker withdraw
  * Maker Generate
  * Curve Stake
  * Curve Claim

Amount of the approved ERC-20 token:

* For safety considerations, the default ERC-20 token amount of approval will be precisely the amount spent on Furucombo.
* You can custom a higher token amount of approval as well. By doing so, before the amount of token approval limit running out, you don't need to send out other approval transactions of the token.
  * MetaMask - when approving Furucombo to spend your tokens, you can click "Edit Permission" to custom a higher spend limit.&#x20;
  * Please note that the transaction will fail if you adjust it to a fewer approval limit.

![Setting Spend limit permission on MetaMask](../../.gitbook/assets/jie-tu-20210304-xia-wu-1.42.39.png)

Examples:

* First-time user Alice's combo: Swap ETH to DAI
  * No need to approve (ETH is not an ERC-20 token)
* First-time user Bob's combo: Swap $500 DAI to ETH
  * Need to approve once for DAI
  * And he adjusts the DAI's Spend Limit on Furucombo to $1000.
* Bob's 2nd combo: Swap $200 DAI to COMBO
  * No need to approve (Because he still has the rest $500 amount of DAI approval limit.)
* Bob's 3rd combo: Deposit WBTC to Maker and Generate DAI
  * Need to approve twice (Once for WBTC, Once for Maker Generate)

### Why does it keep saying my transaction will fail?

In most cases, it's because the price has changed and you need to update the numbers.

If you use flash loan cubes and see the error message, it means that you need to update the numbers of the cubes within the flash loan pair.

### Why did my transaction fail?

In most cases, it's because the price changed which making your combo too far from your original set. You can avoid this kind of failure by leaving more room for slippage:

For example, you want to swap 1 ETH to DAI, then add DAI to Curve pool as a Liquidity Provider (LP):&#x20;

Good combo:

* Cube 1: swap 1 ETH to 400 DAI
* Cube 2: add 380 DAI to Curve pool

Bad combo: &#x20;

* Cube 1: swap 1 ETH to 400 DAI&#x20;
* Cube 2: add 400 DAI to Curve pool

When you enter 400DAI in Cube 2, your transaction will fail once the swapping result in Cube 1 gives you less than 400DAI, which is not uncommon. Leaving a difference in the 2nd cube input can increase the chance of success significantly. In the "Good combo" example, the transaction would only fail when ETH price drops below $380 (> 5%)  between the time you set the combo and send it out.\
\
Using Chained input feature to avoid slippage:&#x20;

* Chained input feature - enabling cubes to auto-capture the previous one's on-chained result to optimize the trading efficiency. With just one click of a "Prev Output" button, you can use 100% entirely swapped amount in a cube to interact instantaneously with your following trading actions.

### Why can't I send even I know it will fail?

It's a mechanism to prevent you from losing money easily.

### How do I cancel my pending transaction?

You can use the "cancel" button in-app if you are using MetaMask or Trust. For other wallets, you can check their official websites for more details. Alternatively, you can also send another transaction with the same wallet and **same** **nonce** with a higher gas price.&#x20;

### My transaction is stuck pending confirmation

In this situation make sure to not keep sending transactions. Every new transaction will be stuck pending until the oldest transaction is confirmed. You can get rid of the stuck transaction by speeding it up or canceling it, depending on if the wallet you are using you has natively that option. For example, Metamask or Trust wallet have both the options to cancel or speed up transactions.&#x20;

Alternatively, if your wallet provider doesn't have a speed-up or cancel option, you can still drop the stuck transaction by sending a 0 ETH transaction to your address (to yourself) using the same nonce (number id). You can inspect the nonce in your transaction on [Etherscan ](https://etherscan.io)and use services like [MEW ](https://www.myetherwallet.com/)and [MyCrypto ](https://mycrypto.com/)to send this transaction with higher gas cost and replace the stuck one.&#x20;

### I can not press the send button

Try to reconnect your wallet.

### I don't know what to build, is there any example combo

Visit [Explore Page](https://furucombo.app/explore) to get some inspirations.&#x20;

### How do I save my combo?

When you set up a combo, click the chain icon underneath the send button. Thank you'll get a link to the current combo.

![](<../../.gitbook/assets/image (20).png>)

### How do I share my combo?

When you set up a combo, there will be a “share” link at the bottom, click the chain icon to get the link or click the Twitter icon to share it on Twitter.

![](<../../.gitbook/assets/image (15).png>)

### I refresh price and it still says it will fail

In most cases, it's because the price changed again and you need to update the numbers.

Furthermore, if you are using 1inch cube and see this error message several times, try to use another swapping cube to get a more stable quotation.&#x20;

### The site does not load

The following steps may solve your problems:

* If you use Brave browser, switch to another browser to discard the issues from the browser. If it is related with Brave browser, some actions to take that may help are:
  * Clearing cache data and cookies for the site
  * Hard refresh with control + F5 (or cmd + r)
  * Disable brave wallet (or the not default wallet been used, for example, metamask, dapper etc)
  * Or other extensions that might be interfering with proper connection with the wallet
  * If after trying all the above steps, it still keeps failing. Unfortunately, we suggest you access Furucombo using other browser as those incompatibilities come from Brave browser.
* Make sure your internet connection is working and is stable
* Restart the browser and try to connect again
* Try to hard refresh the site with control + F5
* Check if there is any update for your browser or wallet provider used, if so, update it to the latest version.

###
