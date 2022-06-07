# Fund Manager Setup

![](../../.gitbook/assets/0\_jrqJPpsrokb\_IDFf.png)

### **Introduction:** <a href="#547e" id="547e"></a>

With the long-awaited [Fund system](https://medium.com/furucombo/introduction-to-furucombo-funds-861926f698ee) launch, we have pushed the opportunity for investment to the next level. Furucombo Fund is an investment platform that matches fund managers and investors on the Polygon network.

As a Fund manager, you can now create your own portfolio on Furucombo. This will demonstrate your trading talent, attract people to invest in your fund, and make use of funds to generate more profit than otherwise would be possible!

For this guide, we will be showing you all the details that you need to know when managing a fund. If you are more of a visual learner, feel free to watch our fund manager workshop video at: [https://youtu.be/DqS80h4p36M](https://youtu.be/DqS80h4p36M).

### **Creating a Fund:** <a href="#d1e5" id="d1e5"></a>

Okay, let’s get started! So how to create a Fund? In the trial run, to maintain the quality of public funds, we won’t yet open the system to the public. You’ll need to submit your information first through this form: [https://forms.gle/4BYF14WFjAbgLdjd9](https://forms.gle/4BYF14WFjAbgLdjd9) to apply for a fund manager role. The Furucombo team will then interview you. After interviewing, we’ll create a fund for you and also a private Discord channel for you to keep in touch with the core team!

The Fund Manager application requires the following information:

`1` Fund name: {Your Fund Name} Fund

* A fund’s name will be shown on the Furucombo invest page and in the contract.

`2` Management fee rate (%):

* A management fee is a pro-rata fee calculated periodically for the assets under a fund’s management and is independent of fund returns paid by fund investors to the fund manager.
* The system will use share tokens as a form of payment tokens.

`3` Performance fee rate (%):

* A performance fee is a pro-rata fee that a fund manager can collect from a fund’s positive return made over a crystallization period.
* The system will use share tokens, charged from fund investors, as a form of payment token to pay off.
* It’ll have a crystallization period as it can reflect more accurately a fund’s overall performance.

`4` Crystallization Period (day):

* The crystallization period is a parameter which can be set by the Vault Manager. Typically it will be set longer than 3 months. The effect of the crystallization period can prevent the performance fee from affecting potential future earnings due to short-term market fluctuations.

`5` Fund owner (wallet address):

* Fund manager’s wallet address — the address that a fund manager uses to open & manage a fund.

**Example:**

1. Fund name: LFG Fund
2. Management fee rate (%): 10%
3. Performance fee rate (%): 10%
4. Crystallization period (day): 100 days
5. Owner (wallet address): 0xeeeeeeeeeeeeeeeeeeeeeeeeeee

### **Fund Interface:** <a href="#9f76" id="9f76"></a>

After being whitelisted in Fund, a “Manage” page will be added to your Furucombo page in the upper-left corner (on the Polygon network). You can easily change the network by clicking the switch. Then, click the “Manage” button, and you can access your private fund page. Once you enter the page, you can see all of your funds under your management.

![Means a fund maintains normal operation.When a fund’s cash balance is negative, it’ll enter an Insufficient period of 72 hours. The fund manager should increase their position in their reserve (USDC) to the fund to get its health factor under control again; otherwise, the fund will be liquidated after the Insufficient period elapses.](../../.gitbook/assets/0\_7y7JcLCAtraYyRMd.png)

Under the ‘Managing Funds’ section, you can select the fund you want to adjust the details of or execute strategies under. Additionally, you’ll find three tabs under your fund’s name: Overview, Strategy, and Setting.

**Dashboard:**

On the overview dashboard page, you can find the following information.

Fund Name: Once you open a fund, you can’t change the fund’s name.

Deposit & Withdraw:

To deposit:

* Hit the deposit button on the upper right of the page.
* Deposit USDC to your fund (currently we only support USDC as the dominant token)
* Manage the fund on the strategy page.

To withdraw:

* To withdraw, simply click the withdraw button to remove the asset from the fund position.

![](../../.gitbook/assets/0\_2R841D4mGJLnB5BT.png)

Performance:

* Contains a chart which will be updated daily, weekly, or monthly.
* Share Price: one share token’s value will vary according to the fund performance

Assets Under Management (AUM):

* Refers to the total market value of the assets that a fund manager handles.

Reserves:

* This shows the amount investors can cash out immediately. If investors want to cash out a higher amount than what’s in reserve, they may need to wait for up to 72 hours & pay a 1% bank run fee.

Status:

* There are four types of status that will be shown.
  * Operating: The cash balance is positive.
  * Insufficient: The cash balance is negative.
  * Liquidating: The cash balance has been negative for over 72 hours, so the fund will be liquidated for all depositors to withdraw.
  * Closed: The fund is no longer in operation and its investors can withdraw their position.

Activeness:

* It’s the ratio to show if the fund manager kept a positive cash balance actively for the past 30 days.

Investors:

* Shows the addresses of investors & the percentage of their portion of the fund.

Portfolio:

* This shows your asset allocation.

About:

* Information: It shows all the information related to your fund.
* Ruleset: It shows all the cubes you can use to create a strategy and manage your fund.
* Investors: It shows the status of your investors — address, share amount and percentage.
* Deposits: It shows all the deposit history of your fund.

**Strategy**:

On the strategy page, you can create a new strategy as well as see all the strategies that you executed. To make a new trade, just hit the ‘New’ button on the upper right of the screen, and it will lead you to a specific create page just for your fund. The page is almost the same as the original create page except for the initial fund section. It’ll show you the value of tokens you’ll receive, and how many cash reserves will remain after using the strategy.

![](../../.gitbook/assets/0\_jSc65HIiX7zcCGFq.png)

**Settings:**

Account & Information:

* Please provide your email address here so that we can give you notices when the status of your funds changes.
* Reserve execution ratio (%): How much percentage of reserve cash does a fund manager need to maintain after executing a strategy.

Fund & Manager Description:

* To attract more people to invest in your fund, you can write some details about your fund strategy. Feel free to write any details that will help you find the right investors to join your fund.

Tracked Assets:

* New assets are automatically tracked when you trade them.

Claimable Fees:

* Fees accrued are automatically settled and paid when depositors deposit or withdraw from your vault. You can also manually claim fees accrued through the Claim button.
  * Management Fee: Refers to the amount of fees you can charge from the funds you manage. You can set this parameter when you create a fund.
  * Performance Fee: Refers to the fees you can collect from the profit you collect. You can set up this parameter when you create a fund.

![](../../.gitbook/assets/0\_UdNu1nwr5itwxQOw.png)

**Furucombo Fees:**

Furucombo will also charge a 0.2% fund fee on each of the transactions performed by the fund manager based on the AUM. For example, if a fund manager performs a swap, and has $10,000 AUM, a 0.2% fee on the $10k AUM will be charged for performing that swap.



🎉 Bravo! You now have the basics to understanding Furucombo’s Fund system! Once you create your own fund, don’t forget to share your fund on Twitter to gain exposure! 🎉



**Contact us:**

If you experience issues that are not covered in this guide, please reach out to the Furucombo team directly via discord.

Website: [https://go.furucombo.app/EjKJD](https://go.furucombo.app/EjKJD)\
Twitter: [https://go.furucombo.app/ouaFR](https://go.furucombo.app/ouaFR)\
Discord: [https://go.furucombo.app/DJ9XF](https://go.furucombo.app/DJ9XF)
