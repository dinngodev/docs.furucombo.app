# Audit Report

Furucombo is composed of [Proxy Contract](https://etherscan.io/address/0xA013AfbB9A92cEF49e898C87C060e6660E050569) & Handler Contracts. We keep conducting audits for all of our Smart Contracts and Handler Contracts to enhance the security of the Furucombo system.

## **Furucombo Audits**

### Website & API **Audit**

The Furucmobo website and API have been audited by [cure53](https://cure53.de/).   
****There were no major or critical issues detected.

{% file src="../.gitbook/assets/fur-01-report.final.pdf" caption="\[cure53\] Website & API audit report" %}

### Furucombo Main Contract

#### Peckshield 

[Peckshield](https://peckshield.cn/en) has formally verified the Proxy, Registry, and handlers of the Furucombo system. Some minor issues were detected which have all been addressed. The full report can be viewed [here](https://github.com/dinngodev/furucombo-contract/tree/master/audit/PeckShield)**.**

#### Certora 

[Certora](https://www.certora.com/) has formally verified the Proxy, Registry, and handlers of the Furucombo system. Some minor issues were detected which have all been addressed. The full report can be viewed [here](https://github.com/dinngodev/furucombo-contract/tree/master/audit/Certora)**.**

### COMBO token and Vesting contracts

#### **C**hainsulting

The COMBO token and Vesting contracts have been audited by [Chainsulting](https://chainsulting.de/).   
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/ChainSulting)**.**

#### Hacken

The COMBO token and Vesting contracts have been audited by [Hacken](https://hacken.io/).   
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/Hacken)**.**

#### **Certik**

The COMBO token and Vesting contracts have been audited by [Certik](https://www.certik.io/).   
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/furucombo-token/tree/master/audit/CertiK)**.**

### **r**COMBO token contract

#### **C**hainsulting

The rCOMBO token ****contract has been audited by [Chainsulting](https://chainsulting.de/).   
****There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/ChainSulting)**.**

#### Hacken

The rCOMBO token ****contract has been audited by [Hacken](https://hacken.io/).   
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/Hacken)**.**

#### **Certik**

The rCOMBO token ****contract has been audited by [Certik](https://www.certik.io/).   
There were no major or critical issues detected. The full report can be viewed [here](https://github.com/dinngodev/RCOMBO/tree/master/audit/CertiK)**.**

### Compound smart wallet handler and Synthetix staking handler

#### **Haechi**

Compound smart wallet handler and Synthetix staking handler have been audited by Haechi with zero critical issues found.

{% file src="../.gitbook/assets/haechi-audit-furucombo-smart-contract-audit-report-v2.0.pdf" %}

{% hint style="info" %}
Furucombo's system DOES NOT hold user's funds right now, so the risk of being hack is relatively low compare to other money protocols. We send user's funds directly to those protocols s/he is using, and we send all funds back to the user's wallet after her/his transaction is done.
{% endhint %}

