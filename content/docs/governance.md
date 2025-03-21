---
title: Governance
description: Learn how to participate in STAB3L governance using rSTB tokens
category: User Guides
order: 3
---

# Governance Guide

STAB3L is governed by its community through a decentralized governance system powered by the rSTB token. This guide explains how to participate in governance decisions and help shape the future of the platform.

## Overview

Governance decisions are made through on-chain voting using the rSTB token. Holding rSTB tokens grants you voting power proportional to your holdings.

The governance system allows token holders to propose and vote on changes to:

- Protocol parameters (fees, rewards, etc.)
- Smart contract upgrades
- Treasury fund allocations
- Partner integrations
- Other platform changes

<div class="mermaid-wrapper">
  <img src="https://quickchart.io/chart?c={type:'flowchart',data:{nodes:[{id:'A',text:'rSTB Token Holders'},{id:'B',text:'Create Proposals'},{id:'C',text:'Vote on Proposals'},{id:'D',text:'Delegate Voting Power'},{id:'E',text:'Discussion Period'},{id:'F',text:'Voting Period'},{id:'G', text:'Implementation'}],edges:[{from:'A',to:'B'},{from:'A',to:'C'},{from:'A',to:'D'},{from:'B',to:'E'},{from:'E',to:'F'},{from:'C',to:'F'},{from:'F',to:'G'}]}}" alt="Governance Flow" />
</div>

## rSTB Token

The rSTB token is the governance token of the STAB3L ecosystem:

- **Total Supply**: 1 billion tokens
- **Token Contract**: `0x...` (ETH), `0x...` (Arbitrum)
- **Token Standard**: ERC-20

### Acquiring rSTB Tokens

There are several ways to acquire rSTB tokens:

Earn rSTB tokens by staking CU tokens:

1. Go to the [Staking page](https://stab3l.io/staking)
2. Connect your wallet
3. Select the CU tokens you want to stake
4. Choose a staking duration
5. Earn rSTB tokens as rewards based on your stake

Purchase rSTB tokens on supported exchanges:

- [Uniswap](https://app.uniswap.org/#/swap) (Ethereum)
- [SushiSwap](https://app.sushi.com/swap) (Arbitrum)
- [Balancer](https://app.balancer.fi/#/trade) (Polygon)
- Centralized exchanges: Binance, Coinbase, Kraken

Earn rSTB tokens by participating in the ecosystem:

- Providing liquidity in the marketplace
- Participating in community activities
- Contributing to the platform development
- Referring new users

## Governance Process

The governance process has several stages:

### 1. Create a Proposal

To create a governance proposal:

1. Hold at least 1,000 rSTB tokens
2. Go to the [Governance page](https://stab3l.io/governance)
3. Click "Create Proposal"
4. Fill out the proposal details:
   - Title
   - Description
   - Changes to be implemented
   - Technical implementation details (if applicable)
5. Submit your proposal

### 2. Discussion Period

After a proposal is submitted, it enters a 3-day discussion period. During this time:

- Community members can discuss the proposal
- The proposer can provide additional information
- Feedback can be incorporated into the proposal

### 3. Voting Period

Following the discussion period, the proposal enters a 5-day voting period. During this time:

- rSTB token holders can vote "For", "Against", or "Abstain"
- Your voting power is determined by your rSTB balance at the time the proposal was created.
- You can split your votes if you have delegated voting power

To vote on a proposal:

1. Go to the [Governance page](https://stab3l.io/governance)
2. Click on the active proposal
3. Choose your vote: "For", "Against", or "Abstain"
4. Confirm the transaction

### 4. Implementation

If a proposal passes, it enters a timelock period (usually 2 days) before implementation. This gives users time to prepare for any changes.

After the timelock period, the proposal is automatically implemented through the governance contract.

## Creating an Effective Proposal

To increase the chances of your proposal being approved, follow these guidelines:

<div class="border p-4 bg-gray-100 rounded-lg">
  <h3 class="font-bold">Proposal Template</h3>
  <p class="text-sm text-gray-500">Requires: 1,000 rSTB</p>
  
  <h4 class="font-semibold">Title</h4>
  <p>A clear, concise title for your proposal</p>
  
  <h4 class="font-semibold">Summary</h4>
  <p>A brief summary of what your proposal aims to achieve</p>
  
  <h4 class="font-semibold">Motivation</h4>
  <p>Why this change is needed and what problem it solves</p>
  
  <h4 class="font-semibold">Specification</h4>
  <p>Detailed description of the proposed changes</p>
  
  <h4 class="font-semibold">Technical Implementation</h4>
  <p>How the changes will be implemented technically</p>
  
  <h4 class="font-semibold">Economic Rationale</h4>
  <p>The economic impact of the proposal</p>
  
  <h4 class="font-semibold">Test Cases</h4>
  <p>How the changes have been tested</p>
</div>

## Governance Parameters

The governance system has several parameters that define how proposals are processed:

- **Proposal Threshold**: Minimum rSTB tokens required to create a proposal (1,000 rSTB)
- **Quorum**: At least 4% of total rSTB supply must vote
- **Majority**: >50% of votes must be "For" for a proposal to pass
- **Discussion Period**: 3 days
- **Voting Period**: 5 days
- **Timelock**: 2 days for standard proposals, 6 hours for emergency proposals

These parameters can be updated through governance proposals.

## Governance Contract

The governance system is implemented through a set of smart contracts:

| Contract | Address | Description |
|----------|---------|-------------|
| Governance | 0x... | Main governance contract |
| Timelock | 0x... | Executes approved proposals after timelock period |
| Treasury | 0x... | Manages protocol funds |
| Proposal Threshold | 1,000 rSTB | Minimum rSTB to create proposal |
| Quorum | 4% | Minimum participation required |

## Delegation

You can delegate your voting power to another address without transferring your tokens. This is useful if:

- You don't have time to actively participate in governance
- You want to support a delegate who shares your vision
- You want to pool voting power with like-minded token holders

To delegate your voting power:

1. Go to the [Governance page](https://stab3l.io/governance)
2. Click "Delegate"
3. Enter the address you want to delegate to
4. Confirm the transaction

You can change your delegation or reclaim your voting power at any time.

## Governance Analytics

The governance dashboard provides analytics on governance activity:

- **Proposal Success Rate**: Percentage of proposals that have passed
- **Voting Participation**: Percentage of rSTB tokens that participate in voting
- **Top Delegates**: Most popular delegation addresses
- **Historical Votes**: Record of past governance decisions

<div class="mermaid-wrapper">
  <img src="https://quickchart.io/chart?c={type:'bar',data:{labels:['Jan','Feb','Mar','Apr','May','Jun'],datasets:[{label:'Voting Participation (%)',data:[28,32,36,42,45,51],backgroundColor:'rgba(54,162,235,0.5)'}]},options:{plugins:{title:{display:true,text:'Governance Participation'}}}}" alt="Governance Participation" />
</div>

## Security Measures

The governance system includes several security measures:

- **Timelock**: Provides time for users to exit if they disagree with a proposal
- **Emergency Cancellation**: Multisig can cancel malicious proposals
- **Guardian Role**: Can pause governance in emergency situations
- **Security Council**: Reviews proposals with smart contract changes

## Community Discussion

Join the governance discussion on our community channels:

- [Governance Forum](https://forum.stab3l.io)
- [Discord #governance channel](https://discord.gg/stab3l)
- [Telegram Governance Group](https://t.me/stab3l_governance)

## Conclusion

Governance is a key aspect of the STAB3L platform's decentralization and development. By holding rSTB tokens and actively participating in governance, you can help shape the future of decentralized compute resources.

For more information on governance, check the [Governance FAQ](https://stab3l.io/faq#governance) or join our community channels. 