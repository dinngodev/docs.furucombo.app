---
description: Furucombo Bug Bounty Program
---

# Bug Bounty Program

### **Program Overview**

The Furucombo team combines the merits of every kind of DeFi protocol to create the most comprehensive DeFi aggregator platform on Ethereum & Polygon. The structure of Furucombo is composed of proxy contracts and handler contracts. The security of our system is of paramount importance to us. While we continue conducting professional audits for the whole system, a bug bounty program is necessary to also ensure the platform’s safety.

This program is intended to work with independent security researchers across the globe and set out our definition of good faith in the context of finding and reporting vulnerabilities, as well as what users can expect from us in return. Should you encounter a security vulnerability in one of our products, we want to hear from you. We believe that the Furucombo ecosystem will be further bolstered with support from our community.

**This bug bounty program is focused on smart contracts and is focused on preventing:**

* Loss of user funds during a transaction by freezing or theft&#x20;
* Loss of user funds by theft of approved smart contracts&#x20;
* Theft of unclaimed yield
* Freezing of unclaimed yield unable to call smart contract&#x20;
* Smart contract gas drainage
* Smart contract failure to deliver promised returns&#x20;
* Interaction with unauthorized handler logic

### **Rewards**

Rewards are distributed according to the impact of the vulnerability based on the [Immunefi Vulnerability Severity Classification System](https://immunefi.com/severity-updated/). This is a simplified 5-level scale, with separate scales for websites/apps and smart contracts/blockchains, encompassing everything from consequence of exploitation to privilege required to likelihood of a successful exploit.

**Smart Contracts and Blockchain Vulnerabilities**&#x20;

* **Critical: Up to 250,000USD**
* **High: 5,000USD**&#x20;
* **Medium: 2,000USD**&#x20;
* **Low: 1,000USD**

All Low, Medium, High and Critical Smart Contract bug reports require a proof of concept to be eligible for a reward.

Critical smart contract vulnerabilities are capped at 10% of economic damage, primarily taking into consideration funds at risk & PR and branding aspects - at the discretion of the team. However, there is a minimum reward of 50,000USD.

Any vulnerabilities found in [https://github.com/dinngodev/furucombo-contract/tree/master/audit](https://github.com/dinngodev/furucombo-contract/tree/master/audit) are not eligible for reward.

FURUCOMBO requires KYC to be completed for all bug bounty hunters submitting a report and requesting a reward. The information needed are name and email address. The collection of this information will be handled by the Furucombo team.

Payouts are handled by the Furucombo team directly, and are denominated in USD. Payments may be done in ETH, DAI, USDC and COMBO, with the ratio at the discretion of the team.

### **Assets in Scope**

**For more information about the scope or eligible contracts, please visit** [**https://immunefi.com/bounty/furucombo/**](https://immunefi.com/bounty/furucombo/)**.**

### Impacts in Scope

Only the following impacts are accepted within this bug bounty program. All other impacts are not considered as in-scope.

#### Smart Contracts/Blockchain

Loss of user funds during a transaction by freezing or theft, loss of user funds approved to smart contracts by theft, theft of unclaimed yield, freezing of unclaimed yield unable to call smart contract, smart contract gas drainage, smart contract fails to deliver promised returns, interaction with unauthorized handler logic

### Out of Scope & Rules

The following vulnerabilities are excluded from the rewards for this bug bounty program:

* Attacks that the reporter has already exploited themselves, leading to damage&#x20;
* Attacks requiring access to leaked keys/credentials&#x20;
* Attacks requiring access to privileged addresses (governance, strategist)&#x20;

#### Smart Contracts and Blockchain&#x20;

* Incorrect data supplied by third party oracles&#x20;
  * Not to exclude oracle manipulation/flash loan attacks&#x20;
* Basic economic governance attacks (e.g. 51% attack)&#x20;
* Lack of liquidity&#x20;
* Best practice critiques&#x20;
* Sybil attacks&#x20;
* Centralization risks

**The following activities are prohibited by this bug bounty program:**

Any testing with mainnet or public testnet contracts; all testing should be done on private testnets. Any testing with pricing oracles or third party smart contracts, attempting phishing or other social engineering attacks against our employees and/or customers, any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks), any denial of service attacks, automated testing of services that generates significant amounts of traffic, & public disclosure of an unpatched vulnerability in an embargoed bounty.

#### Web Vulnerabilities or Out of Scope Issues

Other issues found outside of the locations mentioned above, such as [https://furucombo.app/](https://furucombo.app), will be considered on a case by case basis. Please reach out to the Furucombo development team on [Discord](https://discord.furucombo.app) for clarification.

{% hint style="warning" %}
_Breaking or neglecting any of the rules mentioned above will be a violation of the Furucombo Bug Bounty Program. Furucombo reserves the right to modify or cancel the program at Furucombo’s sole discretion and at any time._
{% endhint %}
