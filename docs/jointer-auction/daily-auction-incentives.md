---
layout: default
title: Daily Auction Incentives
nav_order: 5
parent: Jointer Auction
---

# Daily Auction Incentives
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Jointer provides investors incentives to benefit the group as a whole while still optimizing their own personal benefit. The group is encouraged to outperform the previous day while individuals are incentivized to lead the daily investments and invest the maximum allotted by the Auction on that day. The dual bonus structure provides both large and small investors an opportunity to benefit from the daily success as a group and as an individual.

Both bonuses are uncapped but cannot exceed the daily investment cap.

## Group Discount

The Group Discount is earned through the minting of additional JNTR for distribution. The smart contract increases the number of JNTR minted based on successfully surpassing yesterday's total investment. This allows all investors to benefit from the daily success of a 50% discount and encourages group participation and engagement.

### How the group bonus minted

The daily auction minted supply doubles at a 2:1 rate after the total investment outperforms the previous day's total investment. Minting continues to increase proportionally with more investment, up to the daily investment cap.

**Calculation**

If today's total investment > yesterday's total investment then (((today's total investment /
yesterday's total investment)*2) * baseline supply)

**Example**

If yesterday's total investment was $10,000 and today's total investment stands at $15,000 with a
baseline supply of 10,000 JNTR, the extra supply for the group discount will be 20,000 JNTR
($15,000/$10,000/*2*10,000=30,000).

## Individual Bonus

Investors are incentivized to lead the daily investment round. The bonus is based on their place amongst all investors in the group. The highest discount is based on the highest individual's investment compared to the group. The more individually invested, the greater the individual
bonus.

**Example**

Let's say the final amount of funds invested for a single day is $100,000;

Investor A invested $50,000, Investor B invested $30,000, Investor C $10,000, Investor D $5,000, Investor E $3,000, Investor F $1,500, and Investor G $500.
Based on the individual bonus ranking Investor A receives a 50%[^41]bonus, Investor B receives a 40% bonus, Investor C receives a 30% bonus, Investor D receives a 20% bonus, Investor E receives a 10% bonus, and Investors F and G receive no individual bonus.

### Tie Breaking
In the event two investors invest the same amount, during the same auction day, receiving the same Individual Rank, the rank will go to the investor whose investment was processed first.

**Example**

Let's say the final amount invested for a single day is $100,000; Investor A invests $40,000 which is the first investment processed in the day's auction, Investor B invests $20,000 at the beginning of the Auction and another $20,000 later in the day for a total of $40,000, Investor C $10,000, Investor D $5,000, Investor E $3,000, Investor F $1,500, and Investor G $500.

In this scenario, Investor A and Investor B have tied for first place but Investor A processed their investment first. Therefore, Investor A earns Individual Rank one (1) and receives a 50%[^42] bonus and Investor B earns Individual Rank two (2) and receives a 40% bonus. Further, Investor C receives a 30% bonus, Investor D receives a 20% bonus, Investor E receives a 10% bonus, and Investors F and G do not receive an individual bonus because they have placed outside the Individual Rank.

[^41]: N.B. The 2X includes pro-rata JNTR distribution, the combined Group Discount, and Individual Bonus but does not include the large contribution bonus.
[^42]: N.B. The 2X includes pro-rata JNTR distribution, the combined Group Discount, and Individual Bonus but does not include the large contribution bonus.