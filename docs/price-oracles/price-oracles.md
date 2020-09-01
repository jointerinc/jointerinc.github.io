---
layout: default
title: Price Oracles
nav_order: 8
permalink: /docs/price-oracles
---
# Price Oracles

Since Jointer’s Auction is Ethereum based with currency that is converted in real time to USD face value, the auction smart contract needs an Oracle as a reliable and decentralized source of prices for ETH and USD.

An oracle is a service that provides “trusted” data to smart contracts. Using oracles for token prices is an extremely popular way of fetching
external data through APIs and then utilizing the data as inputs to smart contracts. This process could not be completed with smart
contracts alone, therefore they rely on oracles for such an action (read more from Ethereum on what an Oracle is and how it works [here](https://blog.ethereum.org/2014/07/22/ethereum-and-oracles/).

The following endpoints can be used to fetch the face value USD prices of ETH in various contracts of JNTR/ETN, JNTR/STOCK, and Auction.

- Coinmarketcap
- Any secondary exchange listing JNTR, JNTR/ETN, or JNTR/STOCK
- The Main Jointer Liquidity Reserve
- When prices are from multiple sources [^43] the oracle will calculate the average

![whitelist](/assets/images/oracles.jpg)

### For example, ETH Price

|:-------------|:------------------|
| Coinmarketcap |$207.17 |
| Cointiger | $206.61   |
| STEX | $206.86     |
| HitBtc | $206.50 |
| Median Average Price | $206.78 |

[^43]: This excludes JNTR where the face value price is always derived from the Liquidity Reserve