---
layout: default
title: JNTR/ETN
nav_order: 3
parent: Jointer Syndication Economy
---

# JNTR/ETN
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

![etn](/assets/images/etn.jpg)

JNTR/ETN is a digital asset that acts akin to a bond. JNTR/ETNs are pegged at 2X leverage on the proven Global Select All REIT Index without exposure to the crypto market volatility.

## Historical Data

The Dow Jones Global Select REIT Index is designed to measure the performance of publicly traded REITs and REIT-like securities and is a subindex of the Dow Jones Global Select Real Estate Securities Index (RESI), which seeks to measure equity real estate investment trusts (REITs) traded globally. The index is designed to serve as a proxy for direct real estate investments in part by excluding companies whose performance may be driven by factors other than the value of real estate.

Link to index data (TICKER: DWGRT): (Check Global Select All REIT Index performance [here](https://www.spglobal.com/spdji/en/indices/equity/dow-jones-global-select-reit-index/#overview)

## JNTR/ETN Face Value

The JNTR/ETN initial face value starts at $1 USD and the face value will change at a rate of 2X leverage on the Global Select All REIT Index on a daily basis. Jointer created a smart contract that automatically updates the JNTR/ETN face value which is determined by the daily reporting data provided by the NASDAQ or Dow Jones. The new value JNTR/ETN provides investors coincides with the percentage change of the Index multiplied by the 2X leverage.

**Example**

- Bob invests $100 on January 1, to purchase 100 JNTR/ETN, each day the JNTR/ETN increases or decreases based on the index performance. After one year of holding the JNTR/ETN, the index generates an average return of 10%. Since JNTR/ETN offers 2X leverage the JNTR/ETN face value is calculated as follows: $100 + (10% * 2) = $120

N.B. Jointer deducts a 10% carry from Bob's index profits, therefore going by the above example
Bob's net profit is $118 [read more about [Jointer's Carry](/docs/).

## JNTR/ETN Minting

JNTR/ETN will not be pre-minted, rather it is created based on real time demand when investors
swap to JNTR/ETN using JNTR or JNTR/STOCK.

**Example**

- Bob wants $100 of JNTR/ETN
- So Bob swaps $100 face value of JNTR through the SmartSwap for JNTR/ETN
- A smart contract mints JNTR/ETN at the equal face value of $100 and sends it to Bob

**Example 2**

- Bob wants $100 of JNTR/ETN
- So Bob swaps $100 face value of JNTR/STOCK through the SmartSwap for JNTR/ETN
- A smart contract mints JNTR/ETN at the equal face value of $100 and sends it to Bob

## JNTR/ETN Burning

Similar to how JNTR/ETN is minted, JNTR/ETN is burned each time an investor swaps from
JNTR/ETN to JNTR or JNTR/ETN to JNTR/STOCK.[^28]

**Example**

- Bob holds 100 JNTR/ETN worth a face value of $100
- Bob swaps the 100 JNTR/ETN for JNTR
- Bob receives 100 JNTR
- Jointer's smart contracts automatically burn the 100 JNTR/ETN

## Purchasing JNTR/ETN

Investors have the ability to purchase JNTR/ETN assets in two ways:

1. Through Secondary Market Exchanges
2. Directly from Jointer using SmartSwap


### _Secondary Market_ Exchange
Investors can purchase JNTR/ETN on the open market through secondary market exchanges licensed as Alternative Trading Systems (ATS), National Stock Exchanges such as Merj, or regulated Over-the-Counter (OTC) exchanges.

Investors that buy JNTR/ETN assets are required to go through KYC / AML as well as receive full accreditation checks based on the regulations in the user's governing nation.

### Disclosure:
{: .no_toc }

Jointer respects JNTR/ETN based on a fixed face value of $1 USD plus the changes due to the 2X leverage above the index. Therefore, even if investors buy JNTR/ETN from each other through a secondary market above or below the face value, Jointer still respects JNTR/ETN's value at $1 USD plus the percentage changes due to the 2X leverage index through
SmartSwap.

### Arbitration opportunity
{: .no_toc }

Jointer values all JNTR/ETN equally, regardless of where it was purchased or its purchase price. Investors may utilize secondary market exchanges to purchase their JNTR/ETN below its respective index calculated face value, creating an opportunity for arbitrage buying and selling
between exchanges and Jointer's SmartSwap.

## SmartSwap

The SmartSwap is a decentralized exchange bridge (DEX-Bridge), providing users with two methods to swap, P2P and P2C. Both methods provide trustless swap for digital assets without using a hot wallet while guaranteeing an exact face value match. SmartSwap is precise, low risk,
and 100% fee-free.[^29]

Further, investors are able to swap JNTR/ETN assets using other PP atomic swaps as long as the swap takes place between whitelisted wallets only. Whitelisted individuals will be cleared by Jointer for KYC and AML regulatory requirements and may be subject to other regulations on a country-by-country basis. Any transaction will fail if the receiving wallet is not whitelisted.

### P2P Swap

SmartSwap P2P allows users to generate a transaction ID that can be sent directly to a specific person they want to swap with. Once the transaction ID is created and the users send their digital assets to that transaction ID, the swap will be available only to the counterparty that knows the transaction ID address. Once the swap takes place, the SmartSwap will swap the same face value, if there is any delta it will be returned to the appropriate party.

### P2C Swap

SmartSwap P2C allows users to swap JNTR/ETN with digital currencies without knowing the identity of the counterparty or counterparties. If SmartSwap cannot find a single counterparty to fulfill a transaction it will search for multiple counterparties[^30] to cover the face value and
complete the transaction.[^31] A partial swap is completed first while the rest of the funds remain pending until additional swaps are executed. Users with pending swaps are allowed to cancel the outstanding portion of the swap and receive a refund covering the outstanding amount to the wallet of origin.

**Example**

- Bob wants to swap $1,000 JNTR/ETN with $1,000 BNB
- Bob sends his order to SmartSwap and SmartSwap immediately identifies one counterparty that wants to swap $500 BNB against JNTR/ETN
- In this case, Bob will get the first $500 BNB and the rest of the $500 JNTR/ETN will stay pending until the SmartSwap identifies more counterparties that want to swap BNB with JNTR/ETN

## Selling JNTR/ETN

Ensuring investors have liquidity is at the forefront of Jointer's focus. Keeping with that focus, Jointer will allow investors to sell their JNTR/ETN via SmartSwap or secondary exchange market partners.

### Conversions
Investors are able to sell their JNTR/ETN at any time by swapping the JNTR/ETN to JNTR/STOCK or any other digital assets available (such as JNTR, BNB, ETH, BTC, STABLECOIN, and more). The swap price is calculated based on the current JNTR/ETN face value. The value starts at $1 and is multiplied by the percentage change of the Global Select All REITs Index with 2X leverage.

**Example**

- Bob invests $100 on January 1 to purchase 100 JNTR/ETN at face value of $1 each, over time JNTR/ETN increases or decreases based on the index performance
- After one year of holding the assets, the index generates an average return of 10%
- The JNTR/ETN receives 2X leverage on the 10% index returns
- The new JNTR/ETN face value is calculated as follows: $100 X 110% X 2 = $120 - (Jointer's Carry) = $180
- Bob use SmartSwap to swap the $180 of JNTR/ETN for $180 of BNB

### _Secondary Market_ Exchange
Investors can sell JNTR/ETN via ATS, National Stock Exchanges such as Merj, OTC exchanges, or regulated means to sell securities.

Investors that buy JNTR/ETN assets are required to go through KYC/AML as well as conduct full accreditation checks based on their country's regulation.

Certain jurisdictions regulate securities such as JNTR/ETN making them subject to potential holding periods, locking access to investors' liquidity. For example, the Securities and Exchange Commission (SEC) in the US places a 90 day resale holding period on securities such as JNTR/ETN, which begins after the first JNTR/ETN is sold. The resale holding period for sales to accredited investors, among other conditions, requires that the asset class be in existence for 90 days and will not allow sell orders within this period. Once the 90 day resale holding period ends, investors can go through Jointer's exchange partners to purchase JNTR/ETN from other investors at market rate. Other limitations may also apply depending on the investor's country's regulation.

## JNTR/ETN <> JNTR/STOCK Conversions

JNTR/ETN holders, at any time without limitation, can swap their JNTR/ETN using the SmartSwap at the same face value in return for JNTR/STOCK.

1. If Jointer's Liquidity Reserves hold enough JNTR at the time of the swap, JNTR/ETN holders have the option to swap JNTR/ETN for JNTR at the same face value.

2. If Jointer's Liquidity Reserves do not hold enough JNTR at the time of the swap, the order will remain pending until the order can be executed.

### Swap Without Volatility Exposure

Using SmartSwap, Jointer offers investors a swap between JNTR/ETN and JNTR/STOCK or other digital assets such as BNB and fiat backed stablecoins. Investors that send their order to the SmartSwap will not have exposure to market volatility since the SmartSwap swaps assets with the same face value and without fees or spreads.

### Redemption program

Since JNTR/ETN assets are swappable with JNTR which can be redeemed through Jointer's Liquidity Reserves. Having a swappable asset with JNTR means JNTR/ETN investors indirectly have access to Jointer's Liquidity Reserves.

## Yearly Buyback

As long as Jointer is a private company (complying under Regulation D), shareholder limitations and caps will apply. Therefore, the company may implement a yearly buyback program to clear the CAP table for JNTR/ETN shareholders, if necessary for compliance. Every year before December 31, a buyback event may initiate to comply with Jointer's investors limit (limit set at 2,000 investors per U.S. Regulations).

At the end of the year, Jointer will initiate a swap of all JNTR/ETN assets in exchange for JNTR. At this time, investors have the right to redeem the JNTR assets for other types of value through the reserve (such as digital currencies or stablecoin) that can be sold on a secondary exchange. During the beginning of January, after a short holding period (around 72 hours), Jointer may hold another event where users can swap JNTR back into JNTR/ETN based on the current JNTR market value at that time.

Jointer keeps the right to initiate the swap on a select number of JNTR/ETN holders. In such a case, Jointer will allow the 2,000 largest JNTR/ETN holders to maintain their position if they so choose.

## Taxation

JNTR/ETN is an intangible asset, carrying capital gains tax benefits. JNTR/ETN investors outside of the United States do not need to pay U.S. income tax on their profits. This is unlike REITs or private syndication where investors pay tax on the income distributed. With JNTR/ETN, investors
will only pay capital gains taxes based on the country they associate with. In some countries, investor's profits from JNTR/ETN may end up with zero capital gains tax.

## Target Investors

JNTR/ETN assets are designed for conservative investors because they benefit from cross-collateral and receive returns calculated by providing 2X leverage on the proven Global Select All REIT Index. Those seeking safe exposure to the Commercial Real Estate market, as well as conservative Hedge Funds, Institutional Investors, etc. may see JNTR/ETN as the Jointer asset that best aligns with their needs and the needs of their clients.

## Regulation

From a regulatory perspective, JNTR/ETN is akin to a bond, as such KYC and AML and potentially an accreditation check will be performed on all asset holders. Approved investors wallets will be placed on the whitelist, which will be periodically checked through partner API's to ensure regulations are being met. Once asset holders are whitelisted, they can buy and sell JNTR/ETN.

## JNTR/ETN Quick Facts

- JNTR/ETN is pegged to the Dow Jones Global REIT index with a 2X leverage
multiplier

- There is no pre-mint of JNTR/ETN

- JNTR/ETN's face value changes daily

- JNTR/ETN is purchased only from Jointer through a swap with JNTR

- JNTR/ETN has swap relationships with JNTR/STOCK and other digital currencies

- Jointer can buy back the JNTR/ETN at any given time at the asset's face value

[^28]: Jointer is currently developing a multi-level matching system that will expand instant access to more digital currencies
[^29]:  Gas and transaction fees are reimbursed with Element Zero's native token
[^30]: Multiple counterparties will increase gas costs so the minimum amount of counterparties can be limited by users
[^31]: When there is no buyer in the market, Jointer will step in with JNTR/ETN available to swap
