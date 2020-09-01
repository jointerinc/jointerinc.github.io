---
layout: default
title: Law of Scarcity
nav_order: 2
parent: Jointer's Liquid Economy
---

# Law of Scarcity
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Jointer's main goal is to build a liquid economic structure that naturally creates high demand and low supply in the secondary market. Jointer achieves this goal through fully transparent and automated protocols to create scarcity on the secondary market:

1. Restrain JNTR daily appreciation
2. Daily Contribution Cap
3. 90% JNTR downside protection
4. Network staking
5. Investment power
6. Premium buy-orders
7. Gateway to secondary market

## Restrain JNTR Daily Appreciation

Jointer's longevity and liquidity in the market relies on the Auction to thrive. If JNTR's price appreciates too quickly, investor's would be more apt to sell the JNTR they won at a discount on the secondary market. A deep discount on the secondary market would risk reducing the appeal to investors of participating in the Auction.

Therefore, Jointer created a smart contract that regulates JNTR's daily appreciation in a decentralized manner. The smart contract is not controlled by Jointer and limits JNTR's appreciation to 120% greater than yesterday. When JNTR's appreciation naturally rises above 120%, the Main Reserve transfers the remaining funds to the Side Reserve.

## Daily Contribution Cap

Since JNTR's supply is driven by demand, the total amount of contributions must scale with liquidity in the market. Therefore, not only is the starting JNTR supply low but investments are capped at 150% of the previous day.[^37]

**Example**
On day 2, if the Auction receives $1,000 in investments, the contribution cap on the following auction day cannot exceed $1,500.
(Read more at Maximum Auction Investment)

## 90% JNTR Downside Protection

Jointer presents investors reduced risk investing (Downside Protection) by locking 90%[^38] of their total investment into a smart contract. Only the investor has access to the contract and can cancel at any time, presenting investors peace of mind when investing in Jointer's Syndication Economy.

1. An initial investment for JNTR is received

2. 90% of the investment, along with the JNTR and any group or individual bonuses, will be locked on an escrow smart contract

3. After one year, 90% of the investment will automatically release to Jointer and the assets will release to the investor

4. At any time before the year ends the investor has the option to waive the protection and get the locked JNTR or to cancel the investment and receive 90% of their investment back

**Example**

Assume today's baseline supply is 100 JNTR and the maximum investment is $100
Investor invests 100% of total allotted investment and therefore receives 100% of the daily total supply
The group bonus will increase the supply so the investor receives 200 JNTR
This investor would be eligible for an additional 50% personal bonus of 100 JNTR, bringing their total to 300 JNTR
Because of downside protection, the investor will receive 10 JNTR immediately and the remaining 290 will be locked in Downside Protection along with $90 (90%) of the investment

## Network Staking

Jointer creates a staking incentive network that focuses on building ongoing, mutually beneficial relationships with investors. The other benefit of the network is that it helps achieve Jointer's goal to reduce supply in the secondary market while encouraging investors to unlock their downside protection. Allowing Jointer to invest in Real Estate and add funds to the Liquidity Reserves.

Staking is triggered when investors unlock their downside protection and send their JNTR to a staking contract to receive a daily JNTR award. Investors can choose to unstake their JNTR at any time without restrictions.

By staking their JNTR, investors receive a portion of the total daily minted JNTR. The 1% portion is split into pro-rata portions with other investors choosing to stake. When investors withdraw their JNTR from the staking contract it will include the original JNTR amount plus the accumulated staking award.

### Staking guidelines

- Staking is only available for the locked JNTR in downside protection. Once an investor unlocks their JNTR they can never enroll in the staking program
- Staking rewards are generated on a daily basis and distributed pro-rata between all staking users. Rewards are added to a ledger associated with the user and recalculated daily. The longer users choose to stake, the greater their cumulative pro-rata position
- Daily staking reward amount is paid in JNTR
- Staking simulations produced between 15-50% total potential ROI per year

## Investment Power

Investors must hold JNTR to participate in the daily Auction, effectively placing a hold on selling a relative amount of JNTR as well as increasing buying demand on the secondary market. Investment power is equal to the amount of unlocked/unstaked JNTR held in an investor's wallet.
Investors can invest in Jointer's Auction up to 100% (1:1 face value) of their unlocked/unstaked JNTR holdings at the time of the investment.

If an investor does not have enough investment power to participate in the auction, they will either need to unlock/unstake their JNTR or purchase more from the secondary market or SmartSwap.

**Example**
Investor holds in the wallet $100 worth of JNTR
Investor may invest up to $100 in the auction
Investor will need to unlock, unstake, or purchase more JNTR from other users via the secondary
market to invest more in the Auction

N.B. Investment power will start after day 5 to allow the first investors to become the secondary
market's first sellers.


## Potential Premium Buy-orders

Once a daily Auction achieves the group bonus, which guarantees a 50% discount on JNTR, investors may calculate that they still benefit from paying more for JNTR on the secondary market. Since it is required to have JNTR for investment power, investors will welcome the opportunity to pay a premium to in turn receive an overall net gain.

**Example**
JNTR in the secondary market is $1
The Group Bonus is achieved in the daily Auction
If the investor paid a 20% premium on JNTR in the secondary market to invest in the Auction, the
net profits are as high as 60%
_Calculation - $0.50 Auction profit - $0.20 secondary market premium_

## Secondary Market Gateway

In order to protect the integrity of JNTR's price and protect against a flood of secondary market supply, Jointer placed restrictions on their pre-minted digital assets and the ongoing company supply.

All pre-minted JNTR, JNTR/ETN, and JNTR/STOCK and ongoing JNTR minted as the management fee are restricted from direct access to the secondary market, Liquidity Reserves, SmartSwap, and Atomic Swap.

All Jointer's digital assets under this classification are automatically placed into a digital escrow contract. This contract only allows Jointer's digital assets to be sent to a single address[^39], the Gateway.

The Gateway engages with the secondary market through an API and makes trades based on the calculations of an algorithm which determines market demand. As a result, early investors, founders, providers, and others will receive liquidity without harming Jointer's digital assets face
value.

Once a sell order is completed, the proceeds will be sent back to the escrow to be split pro-rata between the group itself.

![secondary-market-gateway-table.](/assets/images/secondary-market-gateway-table.jpg)

[^37]: Exception is the higher ground rule mentioned below
[^38]: Both personal and individual bonuses are locked in Downside Protection
[^39]: These tokens will eventually be allowed to be transferred to personal storage wallets and family members; the minimum time period is one year.