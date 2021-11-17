---
id: shimmer
title: Shimmer
description: Introduction to the emerging incentivized staging network
keywords:
  - Incentivized
  - staking
  - SMR
---

IOTA Foundation [introduced](https://blog.iota.org/introducing-iota-staking/) Shimmer. An incentivized staging network.
It can be used to work with upcoming IOTA updates before they arrive on the mainnet. It will also have its own token called [SMR](https://shimmer.network/token).
To fairly distribute tokens on the new network, you can stake your IOTA tokens before launch.

## Pre-launch staking

Before the Shimmer network goes online, the IOTA Foundation will announce a start date for "pre-launch" staking.
You will be able to make a transaction to yourself with a certain payload to declare that you want to stake that amount of IOTA tokens to receive SMR. Staking will now be possible for 90 days. You will earn 1 SMR for every 1Mi every 10 seconds.
There is no risk in staking your IOTA Tokens.
Let's take a closer (simplified) look at the technology behind the process.

### Technical overview

Those who are already familiar with the Build/Burn Vote process will recognize the similarities between the Vote and Staking, as it is performed by the same Hornet plugin.  
Hornet operators can enable this plugin. Hornet will then (after a certain milestone) start accumulating all outputs that have the specific Staking payload every 10 seconds. Until the 90 days are up.  
Let's see an example of how this would work:  
Bob has 1Mi on an address that he manages using Firefly, the official IOTA wallet. He wants to use his IOTA tokens to stake for some Shimmer tokens (SMR). He clicks the stake button in Firefly, which generates the transaction to himself with the specific payload. Hornet sees this message and starts accumulating the credit. So after a milestone, the value will be 1 SMR (remember that this token doesn't exist yet. It is just a number in a database). 10 seconds later, after the second milestone, he will have 2 SMR and so on. As long as his IOTA tokens stay on the address he used to stake, he will continue to accumulate SMR tokens.
At the end of the 90 days, Hornet will know how much SMR tokens Bob is allowed to receive on the Shimmer network. This information will then be used to bootstrap the Shimmer network.  
On the Shimmer network, Bob can now claim his real SMR tokens, which are stored at the same address as where his IOTA tokens are stored on the mainnet.  
So the initial amount of SMR is defined by the amount of IOTA tokens staked and for how long they were staked during the 90 days before launch.

## Post-launch staking

On the Shimmer network, you can stake your SMR tokens. An initial APY of 8% is planned. This can be changed later by the community. More information on "post-launch" staking will follow.