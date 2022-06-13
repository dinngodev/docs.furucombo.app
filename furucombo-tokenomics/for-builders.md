# For Builders

> More Builders list their cubes, more profit-discovery combos that Furucombo Masters can create.

As illustrated in Ben Thompson’s [Aggregation Theory](https://stratechery.com/2017/defining-aggregators/), builders make Furucombo more attractive to more users, which in turn draws more builders - in a virtuous cycle.

## The benefit to list a cube on Furucombo

The main challenges for protocol builders in the current DeFi space are often:

* bootstrapping liquidity from scratch;
* the need for interacting with other protocols due to the nature of composability
* lack of front-end resources to provide an intuitive user experience

Furucombo aims to tackle the above problems. To that end, Furucombo emphasizes UX/UI improvements over the protocol layer, whereas the protocol builders can accelerate the development by focusing singularly on the core underlying functionality. This will enable builders to plug-and-play rather than building out their own liquidity.

## The process to list a cube on Furucombo

1. Propose and collect feedback on the [Furucombo Forum](https://forum.furucombo.app/)
2. Pass COMBO Governance on Snapshot
3. Develop the smart contract as per the Cube Listing Policy
4. Submit and schedule the contract review with the Operator (currently the Furucombo founding team)
5. The Operator must register the contract in the system with a multi-sig wallet
6. Lock COMBO to activate the cube

## The security aspect on Furucombo

The overall security of Furucombo is highly related to the DeFis we integrate. Therefore, we need to manage the security from the ground up - that is from the cube development quality and process.

#### Cube Listing Policy

1. Developer Guide: An instruction to build the smart contracts for a new cube on Furucombo.
2. Risk Factors: Different types of cubes will have different risk factors, and different risk factors will be subject to different levels of COMBO commitment and audit processes.
3. COMBO Commitment: To activate a cube on the Furucombo protocol, a certain amount of COMBO needs to be locked in the governance contract as a commitment. Unlocking the committed COMBO will trigger a cool-down period and the respective cube will be delisted immediately.

{% hint style="info" %}
Furucombo Governors with a sufficient amount of vCOMBO could commit to activating a cube. Additionally, the committed party could still participate in the governance and enjoy the benefit as a Governor.
{% endhint %}

#### Regular Audit

Furucombo Operator (currently the Furucombo founding team) will schedule and conduct regular internal and external audits to ensure more and more experienced experts examined the code along with the growth of the protocol.

#### Insurance Policy

When a cube performs malicious behavior, the committed COMBO will be taken and sent to Furucombo Reserve, and the Operator will delist the cube from the system immediately.

On the other hand, Furucombo Governors can allocate the funds in the Furucombo Treasury to underwrite or buy insurance from external insurance protocols for the overall users.

## Example on how to participate as a Builder

#### Before your cube gets listed:

1. Propose your cube idea on the [Governance Forum](https://forum.furucombo.app).
2. Interact with other members of the community to gather support.
3. Find a Governor who supports your idea to create a cube listing proposal, or you can get enough vCOMBO to be a Governor yourself and create the listing proposal.
4. If the proposal is passed with support from the Governors, you can then develop the smart contract per the Cube Listing Policy.
5. Once the contract is ready, submit and schedule the contract review with the Operator (currently the Furucombo founding team)
6. If the review is positive, the Operator will register the contract in the system with a multi-sig wallet.
7. Then you need to purchase COMBO tokens from open market. For example, you can [buy COMBO from Uniswap](https://furucombo.app/combo/c3gnmecke6ss71ddm290). Then, you need to lock these COMBO tokens into the COMBO locking contract to activate the cube. You can also seek support from the Furucombo governance beforehand to see if any sponsors from the community.

#### After your cube gets listed:

1. As you lock the COMBO, you also become a Furucombo Governor. You are encouraged to participate in the COMBO governance actively going forward.
2. With the rapid development in the DeFi space, its recommended to follow up on the DeFi cube you develop from time to time. For example, when the underlying DeFi has an upgrade, you may need to upgrade the cube to make it functional as well.
3. You can apply for grants from the Furucombo Governance Portal as your cube accumulates transacted volume.

## Release Schedule

{% hint style="info" %}
Due to the nature of the DeFi space, expeditated development, unforeseen changes, or community feedback may cause these plans to change.
{% endhint %}

| Subject                                                                                               | Status    |
| ----------------------------------------------------------------------------------------------------- | --------- |
| [Smart Contract Open Source](../resources/deployed-contracts.md#proxy-contract)                       | Completed |
| Trial Run on External Builder Participation ([Sushiswap and B.Protocol](https://furucombo.app/combo)) | Completed |
| Cube Listing Policy                                                                                   | Planning  |
| Cube Stats Dashboard                                                                                  | Planning  |
| Smart Contract for Cube Activation                                                                    | Planning  |

