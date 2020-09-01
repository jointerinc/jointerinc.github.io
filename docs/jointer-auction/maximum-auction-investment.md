---
layout: default
title: Maximum Auction Investment
nav_order: 2
parent: Jointer Auction
---

# Maximum Auction Investment
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Daily, during Auction hours, investors have the opportunity to invest as much or as little as they desire as long as the total investment, from all investors combined, does not exceed the maximum investment allowed, which is 150% of the previous day's investment amount.

## Higher Ground Minting Rule

Since the daily maximum contributions are directly tied to auction performance, Jointer needs to set an exception rule for unexpected investment behavior. Therefore, when yesterday's total investments are lower than the total investment of the day prior to yesterday, Jointer takes the average of the previous 10 days of investments when deciding the new maximum amount.

Formula
If yesterday's investment is higher than the day before yesterday than:
Yesterday's total investment * 150%

If yesterday's investment is lower than the day before yesterday than:

The average calculation of 10 Days = (Total investment in the last n days) / n days * 150%

N.B. The smart contract uses whichever calculation is higher.

Example
Yesterday's total Investment = $10,000
Total investment of the day before yesterday = $25,000
(10 day average = $23,586) * 150% = Today's max investment $35,379