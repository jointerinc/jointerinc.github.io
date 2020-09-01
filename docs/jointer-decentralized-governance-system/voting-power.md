---
layout: default
title: Voting power
nav_order: 1
parent: Jointer Decentralized Governance System
---

# 1. Voting power
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Individual users gain voting power by holding JNTR. The cumulative individual voting power is how majority level decisions are either affirmed or denied.

### How voting power is determined

1. Equal weight is given to all JNTR, no matter where or when they are purchased
2. Each user holding JNTR in their wallet receives voting rights
3. 1 JNTR = 1 vote
4. JNTR must be unlocked and unstaked to receive voting power (i.e., JNTR locked or staked through the protocol will not count as a vote)
5. Pre-minted JNTR has the same rights as any other JNTR


### What is cumulative individual voting power (CIVP)?

A user's cumulative individual voting power (CIVP) is their combined JNTR across all their wallets. This means as long as a wallet is linked under a specific user's account they will be cumulatively counted (a user's CIVP counts only unlocked and unstaked JNTR across all their wallets).

Some rule alterations require different types of Majority Levels and users can use their CIVP to influence the outcome of the rule proposal by voting YEA or NAY.

At the time of voting, the DGS snaps and timestamps the current cumulative JNTR per user. At the close of the vote, the DGS will re-snap and timestamp users' CIVP to protect system integrity in the case that a user's CIVP changes during the open voting process.

**Example**

User A has three (3) wallets that hold JNTR

Wallet one (1) has 4,000 unlocked JNTR and 2,000 staked JNTR

Wallet two (2) has 2,000 unlocked JNTR

Wallet three (3) has 3,000 JNTR locked in Downside Protection

When the DGS snaps and timestamps to initiate a voting window, User A will have 6,000 votes (Wallet one (1): 4,000 + Wallet two (2): 2,000)

The staked JNTR in Wallet one (1) and locked JNTR in Wallet three (3) do not count towards User A's CIVP
