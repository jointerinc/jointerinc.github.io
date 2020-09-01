---
layout: default
title: Whitelist
nav_order: 9
has_children: true
permalink: /docs/whitelist
---

# Whitelist

A whitelist is implemented to allow Jointer’s smart contracts to interact only with approved addresses. This means only whitelisted addresses
can receive Jointer’s digital assets. In this case, a transaction will take place only if the wallet holders have passed necessary KYC and AML, or any other verifications needed, and is part of the whitelist.

![whitelist](/assets/images/whitelist.jpg)

- Jointer maintains one whitelist for each individual Jointer digital asset and a whitelist processor updates the whitelists.
- Once a wallet is added to any of the whitelists, it is unable to be removed meaning it can always swap Jointer’s assets.
- The whitelist processor can block wallets that no longer meet AML/KYC or other terms of use from receiving new digital assets.
- If investors purchase Jointer’s digital assets through third-party exchanges, the investors' wallet address is automatically added to the associated whitelist once approved by the third-party exchange.
- Third-party exchanges provide Jointer a list of wallets that are not compliant with KYC/AML, allowing Jointer to use the whitelist processor to block the wallet from purchasing new Jointer’s assets.
- During Jointer’s Auction, every investor is whitelisted based on their KYC/AML and possible accreditation which is checked through third-party providers and updated on-chain within the Jointer system.
- Investors from regulated countries will need to pass a full accreditation check.
- The Jointer system will periodically check the whitelists with KYC/AML providers against the existing investors and update accordingly.
- Frequency of checking KYC/AML with providers is configurable from the Jointer Admin System.