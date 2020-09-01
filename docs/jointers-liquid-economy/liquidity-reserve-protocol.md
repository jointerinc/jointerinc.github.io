---
layout: default
title: Liquidity Reserves Protocol
nav_order: 1
parent: Jointer's Liquid Economy
---

# Jointer's Liquidity Reserves' Protocol
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

Jointer's Liquidity Reserves are powered by multiple smart contracts creating multiple reserves and tiers of decentralized rules on top of Bancor's relay protocol. The Reserves are funded with 10% of all investment received to support everlasting liquidity for investors and JNTR's
sustainability. In accomplishing these goals, Jointer utilizes a Main Reserve, a Side Reserve, a Turnover Reserve, and an Overflow Reserve.

All Liquidity Reserves are fully decentralized, without any interference from Jointer or any other centralized party.

## The Main Reserve

The Main reserve has two responsibilities, one is to provide ongoing liquidity for JNTR holders when they redeem their JNTR and secondly to calculate JNTR's face value.

To establish Jointer's Main Reserve, Jointer uses the Bancor relay protocol to store funds and JNTR into two pools that act as a fractional reserve for redemption. One pool holds JNTR and the other pool holds BNT. Every time BNT or JNTR is added or removed from their respective pools,
the JNTR face value will change. Therefore, when BNT is added to the pool, JNTR is removed from the other pool. As a result, JNTR's face value increases. Conversely, if JNTR is added to the pool, BNT is removed from the other pool and as a result, JNTR's face value decreases.

### Main Reserve Funding
The Main Reserve consistently receives up to 3% of the total Jointer Auction investment as well as splitting surplus funds from the Side Reserve.

### Main Reserve Redemption Recovery
Every time users deposit JNTR through the Main Reserve, the Side Reserve recovers the Main Reserve to keep JNTR's face value the same even after the redemption. The automated process uses digital currency in the Side Reserve to swap with the Main Reserve for the redeemed JNTR.

### Financially Engineered Calculation of JNTR's Face Value
JNTR's face value changes with every currency deposited to pool A or when JNTR is purchased from pool B. Therefore, the ratio between pool A and pool B determines JNTR's face value.

**Example of JNTR Redeemed**

Pool A has a $100 value of digital currency and pool B has 100 JNTR.

The value of JNTR is $1 based on pool A/pool B (100/100).

If 2 JNTR are redeemed (meaning deposited into pool B in exchange for funds from pool A), the first JNTR will be redeemed at $1.

Subsequently, the pools recalculate the ratio, which is now $99 in pool A and 101 JNTR in pool B.

Therefore, JNTR's new face value is $0.98 (99/101).

The second JNTR will be redeemed at $0.98.

After this redemption, the pool ratio changes to $98.01 in pool A and 102 JNTR in pool B.

So after the 2 JNTR are redeemed, the new JNTR face value is $0.96.

**Example of Digital Currency Deposit**

When Jointer Liquidity Reserve Protocol sells JNTR, it uses the digital currency allocated to the Main Reserve to purchase JNTR from pool B and deposit funds to pool A. This automated action increases JNTR's face value relative to the new ratio between pool A and pool B.

### Face Value Restoration

Since JNTR's face value is derived from the Main Reserve and investors redeem from this reserve,
it is important the Main Reserve maintains liquidity. Therefore, the Main Reserve is replenished
by the Side Reserve. If two orders are placed simultaneously, the side reserve is responsible for
refilling the main reserve between each order to the exact same face value it was before the first
redemption

**Example**

100 JNTR are deposited to the Main Reserve(as part of the redemption process)
The Side Reserve has available funds so it withdraws 100 JNTR from the Main Reserve, restoring
the Main Reserve's exact previous face value.

### Protection against manipulation and volatility

Since the face value of JNTR relies on pool A which holds BNT in the Main Reserve, there must be protections against market manipulation or volatility. If protections were not in place, JNTR would be altered in an unreasonable manner every time BNT changes value or each time someone sends funds directly to pool A to the blockchain address. Therefore, Jointer implemented an automated process to ensure neither potential reality could harm JNTR's
integrity.

**BNT increases in value**

- Every time BNT increases value, the smart contract triggers relative pool liquidation (using the Relay ownership tokens) from both pool A and pool B to keep the ratio the same. The pool liquidation amount is equal to the volatility percentage change.
- After liquidation, the smart contract redeposits JNTR back to pool B and sends the BNT to the Turnover Reserve.
- This process balances the JNTR face value to the original position before the BNT value increased.

**BNT decreases in value**

- Everytime BNT decreases value, the smart contract triggers relative pool liquidation (using the Relay ownership tokens) from both pool A and pool B to keep the ratio the same.
- Each pool's liquidation amount is equal to the volatility percentage change.
- After liquidation, the smart contract redeposits BNT into pool A and sends JNTR to the
- Overflow Reserve.
- This process balances the JNTR face value to the original position before the BNT
decreases.

**Direct deposit to pool A**

- Every time there is a direct deposit to pool A, the smart contract triggers relative pool liquidation from both pool A and pool B to keep the ratio the same.
- After liquidation, the smart contract redeposits JNTR back to pool B and sends the BNT to the Turnover Reserve.
- This process balances the JNTR face value to the original position before the direct deposit to pool A.

**Direct deposit to pool B**

- Pool B is protected by a smart contract that prevents any JNTR deposits outside the Jointer system.

## The Side Reserve

The Side reserve has two responsibilities, to recover the Main Reserve which protects JNTR's face value, and provide excess funds to the Main Reserve to increase liquidity depth. Funds are not directly withdrawn from the Side Reserve by investors, rather the Side Reserve communicates
directly with the Main Reserve and refills the Main Reserve after redemptions.

The Side Reserve protects JNTR's face value from decreasing in the Main Reserve by providing digital currency for the redeemed JNTR in the Main Reserve. The Side Reserve increases liquidity depth by pushing surplus Side Reserve digital currency to the Main Reserve in exchange for
JNTR.

### Side Reserve Funding
The Side Reserve consistently receives at least 7% of the total Jointer Auction investment.

### Side Reserve Refill
Since the Side Reserve is used to recover redemptions from the Main Reserve, there may come a
time when the reserve falls short. If the Side Reserve is unable to recover the Main Reserve
completely, the Turnover Reserve will refill the Side Reserve to allow it to complete this process.

## The Turnover Reserve

The Turnover Reserve acts to automatically and responsibly refill the Side Reserve.

### Turnover Reserve Funding
The Turnover Reserve receives 10% each time investors purchase JNTR through channels other than the auction, such as purchasing JNTR from the protocol for JNTR/ETN or JNTR/STOCK.

### Turnover Reserve Triggers
The Turnover Reserve has two triggers that spring it into action. One, to refill the Side Reserve when it is empty and two, to initiate the Relay ownership token to liquidate the main reserve pool.

## The Overflow Reserve

The Overflow Reserve Protocol purchases JNTR throughout different processes included in the multiple reserves. The Overflow Reserve holds all of these JNTR and uses them to create liquidity and to regulate the Main Reserve.

### Overflow Reserve Funding
The Overflow Reserve receives funds from two sources, the main reserve and from investors
swapping JNTR through SmartSwap.

First, the Overflow Reserve receives JNTR from the Main Reserve every time the Main Reserve uses digital currency to purchase JNTR from the pool. Second, JNTR is added to the Overflow Reserve everytime investors swap JNTR for JNTR/ETN or JNTR/STOCK.

### Overflow Reserve Triggers
When the Overflow Reserve runs out of JNTR, it will trigger the relay ownership token to liquidate
the Main reserve and refill the Overflow reserve with JNTR.

## Relay Ownership Tokens

The Relay Ownership tokens represent ownership of the two pools in the Main Reserve. The holder of the relay has the ability to redeem up to 100% of the currency from the Main Reserve pools. The Liquidity Reserve protocol utilizes the Relay token to partially liquidate, from both Main Reserve pools, creating a decentralized circuit breaker that does not affect the JNTR face value.

Relay Ownership token responsibilities include:

1. Recovering the Turnover reserve and the Overflow reserve.
2. Stabilizing JNTR face value against market volatility and price manipulation.
a. **Increase in currency market price -** When the digital currency (Bancor's BNT) market value in pool A increases, the value of the entire pool increases. So if the currency
increases by 10% the value of pool A would increase from $100 to $110. Without the Relay Ownership token, the value of JNTR, which is determined by pool A, would
increase. Because of the Relay Ownership token the crypto market price volatility never affects JNTR's face value.

Jointer accomplishes this by automatically redeeming 10% from both pool A and pool
B, then depositing back into pool B enough JNTR to return it's face value to its starting
value before the 10% currency market price increase.

b. **Decrease in currency market price -** When the digital currency (Bancor's BNT) market value in pool A decreases, the value of the entire pool decreases. So if the currency decreases by 10%, the value of pool A would decrease from $100 to $90.Without the Relay Ownership token, the value of JNTR which is determined by pool A, would decrease. Because of the Relay Ownership token, the crypto market price volatility never affects JNTR's face value.

Jointer accomplishes this through automatically redeeming 10% from BOTH pool A and pool B, then depositing back into pool A enough currency until the face value of JNTR reaches it's starting face value before the 10% currency market price depreciation.

c. **User manipulation -** If Jointer's system were to receive funds directly into pool A from an attacker looking to manipulate the JNTR face value, the system process compensates by redeeming an equal % of the manipulated JNTR from the relay in an equal amount from both pool A and pool B. Then the Liquidity Reserve process deposits enough JNTR into pool B until the face value of the JNTR returns to its initial face value before the attack.

## Liquidity Reserve Redemptions

Investors are able to access the on-chain Liquidity Reserves through the Jointer web portal. The portal allows users to interact with the Reserves without needing a counterparty for a trade.

### Infinite liquidity with slippage

Slippage is traditionally used to provide price discovery without a counterparty but the price discovered may not be the exact price at which the trade is executed because of slippage. The slippage on a trade is the variance between the expected price which is discovered before the transaction is executed and the final, exact price at which the trade executes.

Depending on the size of the trade and the available liquidity, each transaction will have different slippage. The larger a given withdrawal is compared to the liquidity in the pools, the higher the price slippage on the transaction will be.

From a mathematical perspective, this makes the liquidity unlimited and provides the ability to restore JNTR's face value after any event. The entire process is automated and processed on public blockchains which means JNTR's face value can increase value but can never decrease.

### Price slippage recovery

Jointer financially engineered the Reserves to provide a perfect price slippage recovery for investors which goes beyond the simple slippage model. Utilizing the Side Reserve to consistently recover the Main Reserve after a redemption of JNTR provides price slippage recovery for the next investor wanting to redeem JNTR.

**Example**
The Main Reserve executes a redemption request reducing the digital currency in pool A while adding JNTR to pool B, which traditionally increases the slippage for the next investor After the trade is executed, the Side Reserve withdrawals the same amount of JNTR from pool
B to the Side Reserve
The Side Reserve withdrawal brings the face value to the original position before the redemption and decreases the slippage back to the initial value before the redemption
Therefore, the next investor is not damaged by the investor redeeming JNTR first as they both receive the same slippage calculation

N.B. JNTR's face value recovery takes place between displays to avoid quick trading investors or API players who may abuse the temporary face value change. This means, the volatility due to redemption is recovered by the Side reserve in a way that is transparent to the public.

### Continuous liquidity during zero investment

Even in a scenario where no reserve allocation is received because there is zero auction investment, the contribution trigger will initiate an automatic process to provide funds to the Main Reserve.

If the Side Reserve has enough funds it will contribute to the Main Reserve up to 1:1 value of yesterday's Main Reserve Contribution amount.

If the side reserve does not have enough funds to contribute to the Main Reserve, the Turnover will recover the Side reserve. Similarly, if the Turnover does not have enough funds to recover the Side reserve, the Turnover Reserve will automatically trigger the Relay ownership token to liquidate 10% of the Main pools.[^36] The process takes 10% of the proceeds from liquidation to push capital to the Turnover Reserve, which in turn refills the Side Reserve, allowing it to follow normal processes and directly contribute up to 1:1 value of yesterday's Main Reserve Contribution amount.

The contribution trigger allows continuous liquidity and growth even without Auction investment.

### Matching Contributions

Every time the Side Reserve has extra funds it uses the funds to match original contributions to the Main Reserve at a 1:1 ratio. This method, also referred to as tag along contributions, is designed to increase the liquidity in the Main Reserve cautiously and responsibly, following the organic demand and making sure not to disproportionality boost the face value of JNTR.

### Mirror the Federal Reserve's Economic Psychology
As mentioned above, JNTR was financially engineered to set a face value floor and constantly increase. Therefore, much like the Federal Reserve Gold system used to back currency, economic psychology plays a role in secondary trading.

The psychology assumes that the secondary markets will follow closely to JNTR's face value in the Liquidity Reserve. This is similar to the old Federal Reserve Gold system to back currency because although the gold is not physically traded, the paper currency receives a denomination as if it were and it is traded on secondary markets following this mindset. This same concept applies to Jointer's Liquidity Reserves and Syndication Economy. JNTR's face value can be trusted since there is an option to redeem for digital currency from the Liquidity Reserve process, just like theFederal Reserve.

For example, if the system offers JNTR redemptions for $1 and after a few days the ratio in the reserve increases, pushing JNTR's face value to $2, it is unlikely that JNTR will trade on secondary markets for a value that deviates far from $2. When the number deviates enough, an arbitrage opportunity arises creating incentive to close the difference between the two values.

So in other words, Jointer's Liquidity Reserves allow the public the ability to enjoy from JNTR's growth with decentralized mechanisms that once a floor is established, the face value cannot drop below it, while being supported with unlimited liquidity.

### Arbitrage Pricing Theory

As well as benefiting from the Liquidity Reserves, JNTR's secondary market value will also utilize the Arbitrage Pricing Theory. The theory holds that an asset's expected return allows sophisticated investors to recognize discounts which allows them to increase their rate of return on an investment.

Therefore, since JNTR is a way of payment to purchase JNTR/STOCK and JNTR/ETN investors calculate that they receive a higher rate of return by purchasing discounted JNTR in the secondary market. Purchasing JNTR at a discounted rate and using it to purchase JNTR/ETN or JNTR/STOCK, investors receive real estate backed assets for a fraction of the face value.

[^36]: Liquidating relay tokens reduces the numerator and denominator of total available tokens in the pool and Jointer assets equally by 10% without changing the token value or token ratio. Learn more about Bancor rally tokens:
https://support.bancor.network/hc/en-us/articles/360000471472-How-do-Relay-Tokens-work-

