# Audit Report

Furucombo is composed of [Proxy Contract](https://etherscan.io/address/0xA013AfbB9A92cEF49e898C87C060e6660E050569) & Handler Contracts. We keep conducting audits for all of our Smart Contracts and Handler Contracts to enhance the security of the Furucombo system.

## **Furucombo Audits**

### Furucombo Main Contract

#### Peckshield&#x20;

[Peckshield](https://peckshield.cn/en) has formally verified the Proxy, Registry, and handlers of the Furucombo system. Some minor issues were detected which have all been addressed. The full report can be viewed [here](https://github.com/dinngodev/furucombo-contract/tree/master/audit/PeckShield)**.**

#### Certora&#x20;

[Certora](https://www.certora.com/) has formally verified the Proxy, Registry, and handlers of the Furucombo system. Some minor issues were detected which have all been addressed. The full report can be viewed [here](https://github.com/dinngodev/furucombo-contract/tree/master/audit/Certora)**.**

### Website & API **Audit**

The Furucmobo website and API have been audited by [cure53](https://cure53.de/). **** \
****There were no major or critical issues detected.

{% file src=".gitbook/assets/fur-01-report.final.pdf" %}
\[cure53] Website & API audit report
{% endfile %}

### **Furucombo Smart Wallet & Auto-Farming Feature Contract**

**Peckshield** \
\
The Furucombo smart wallet and auto-farming feature contract have been audited by [Peckshield](https://peckshield.cn/en). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-smart-wallet/tree/master/audit/PeckShield)**.**

#### Dedaub&#x20;

The Furucombo smart wallet and auto-farming feature contract have been audited by [Dedaub](https://www.dedaub.com/). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-smart-wallet/tree/master/audit/Dedaub)**.**

### **Furucombo Trevi System Contract**

#### **C**hainsulting

The Furucombo Trevi system contract has been audited by [Chainsulting](https://chainsulting.de/). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/trevi/tree/master/audit/Chainsulting)**.**

#### HashCloak

The Furucombo Trevi system contract has been audited by [HashCloak](https://hashcloak.com/). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/trevi/tree/master/audit/HashCloak)**.**

#### Peckshield&#x20;

The Trevi system contract has been audited by [Peckshield](https://peckshield.cn/en). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/trevi/tree/master/audit/PeckShield)**.**

### COMBO token and Vesting contract

#### **C**hainsulting

The COMBO token and Vesting contracts have been audited by [Chainsulting](https://chainsulting.de/). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/ChainSulting)**.**

#### Hacken

The COMBO token and Vesting contracts have been audited by [Hacken](https://hacken.io/). \
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/Hacken)**.**

#### **Certik**

The COMBO token and Vesting contracts have been audited by [Certik](https://www.certik.io/). \
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/CertiK)**.**

### **r**COMBO token contract

#### **C**hainsulting

The rCOMBO token **** contract has been audited by [Chainsulting](https://chainsulting.de/). **** \
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/ChainSulting)**.**

#### Hacken

The rCOMBO token **** contract has been audited by [Hacken](https://hacken.io/). \
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/Hacken)**.**

#### **Certik**

The rCOMBO token **** contract has been audited by [Certik](https://www.certik.io/). \
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/CertiK)**.**

### Compound smart wallet handler and Synthetix staking handler

#### **Haechi**

Compound smart wallet handler and Synthetix staking handler have been audited by Haechi with zero critical issues found.

{% file src=".gitbook/assets/haechi-audit-furucombo-smart-contract-audit-report-v2.0.pdf" %}

{% hint style="info" %}
Furucombo's system DOES NOT hold user's funds right now, so the risk of being hack is relatively low compare to other money protocols. We send user's funds directly to those protocols s/he is using, and we send all funds back to the user's wallet after her/his transaction is done.
{% endhint %}
