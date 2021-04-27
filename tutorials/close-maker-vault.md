---
description: 'Tutorial: Close Maker vault'
---

# Close Maker vault

![](https://miro.medium.com/max/6400/1*MH_gQLHLVVkm_geXKVldEQ.jpeg)

In this article, we will walk you through what is Liquidation and a strategy on how to avoid getting liquidated. For this strategy, you can use it to close the Collateralized Debt Position \(CDP\) when something goes wrong suddenly, and you can use it to realize the leverage DAI profit as well.

If you are not familiar with Maker vault, you can read our [previous article](https://docs.furucombo.app/tutorials/boost-maker-vault) first to know what Maker vault is and how to open one!

## **What is Liquidation on Maker?** <a id="d9e4"></a>

Liquidation is the process of selling collaterals to repay the amount of DAI a user has generated from their vault. When the vault’s Collateralization Ratio falls below the required minimum level \(Liquidation Ratio\), the vault position would be automatically liquidated through a collateral auction. To put it simply, when the price of your collateral slumps, you might lose all of the assets in the vault. Maker’s Liquidation process can reduce the DAI debt in circulation to ensure that DAI could always be backed by an appropriate amount of collaterals to maintain DAI’s price.

### What happens during a Liquidation? <a id="191d"></a>

When a vault breaches its Liquidation Ratio, Maker Keeper triggers the Liquidation process. All collaterals in this vault are put up for auction to be sold to pay back the outstanding DAI, the 13% liquidation penalty, and the stability fees. Once the auction completes, the bidder receives the sold collateral, and the vault owner gets the remaining collateral if there is any.

## **How to avoid getting liquidated?** <a id="78fe"></a>

When collateral price becomes volatile and close to the Liquidation Price, the vault owner may deposit more collateral or pay DAI back into the vault to raise its Collateralization Ratio to prevent it from getting liquidated. To increase the vault’s Collateralization Ratio, you may go to [Maker Oasis Barrow](https://oasis.app/borrow), or even better, you use [Furucombo](https://furucombo.app/combo)! Just go to the menu and select “Deposit” or “Pay Back” under the Maker section. There is yet another ultimate way that can be used to avoid the Liquidation called Self-Liquidation.

![Pay DAI back into the vault to raise its Collateralization Ratio](https://miro.medium.com/max/5760/1*V7uhiRzS0pZuGo-CjdfSIA.png)

## **What is the Self-Liquidation strategy?** <a id="7099"></a>

The concept of the Self-Liquidation strategy is to repay the loan and close the vault in advance if something suddenly goes wrong. Just simply think of this strategy as closing your Collateralized Debt Position \(CDP\) completely. The approach is to sell the collaterals and pay off all the debts, and the trick is how to do it when your collaterals are locked. Easy. Do it with flashloan.

## **How to build this strategy?** <a id="3497"></a>

There are two ways of building this strategy:

* Basic level: Build Manually with Flashloan as upfront funds
* Pro level: Skip building. Just use Furucombo’s latest feature on the [Explore Page](https://furucombo.app/explore/combo_maker_00001).

### **1\) Basic level: Build manually with Flashloan**

```text
Step 1: Borrow DAI from Flashloan
Step 2: Pay off all the debts
Step 3: Withdraw all the collateral to close the vault
Step 4: Swap the collateral to DAI
Step 5: Repay Flashloan with fee
*You will get the remaining collaterals back to your wallet.
```

![Build Manually with Flashloan to close Maker vault](https://miro.medium.com/max/5760/1*1IuJuix79aybPyzJgXmXEg.png)

### **2\) Pro Level: Skip building**

Furucombo has simplified all the Basic level steps into a [setup form](https://furucombo.app/explore/combo_maker_00001). Thus, you can Self-Liquidate your vault with ease by selecting the vault number you want to close the position. In the setup form, you can clearly see the vault’s before-and-after changes. The Output number in the setup form means how much collaterals you’ll get back to your wallet after self-liquidating.

```text
Step 1: Select vault number
Step 2: Approve & Send the transaction
*You will get the remaining collaterals back to your wallet.
```

![Pro Level: Skip building](https://miro.medium.com/max/5760/1*lUkIDBTvinCsX3kdNydedg.png)

### **Another timing of using the Self-Liquidation strategy**

When DAI’s price is higher than stablecoins’ price \(USDC, USDT, TUSD\), you could create a new vault using stablecoin as collateral and generate more DAI to leverage your position \(You can follow [this article](https://medium.com/furucombo/tutorial-boost-maker-vault-3faf01db2a55) to increase your vault’s exposure easily\). And when the DAI’s price closes to the collateral’s price again \(or even lower than the collateral’s price\), at this moment, you can execute the Self-Liquidation strategy to close your vault and to realize the leverage DAI profit!

Here’s a case study:

{% embed url="https://twitter.com/furucombo/status/1288837013634838528?s=20" %}

_🎉 Bravo! You’ve closed your Maker vault. Don’t forget to share your result on Twitter. 🎉_

![](../.gitbook/assets/1_rqjs5y9tpgufzxczib5qbg%20%282%29.gif)

