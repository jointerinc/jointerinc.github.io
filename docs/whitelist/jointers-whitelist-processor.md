---
layout: default
title: Jointer's Whitelist Processor
nav_order: 1
parent: Whitelist
---

# Jointer's Whitelist Processor

Jointer developed a protocol layer on top of the traditional whitelist structure which allows authorizations and limitations on wallet addresses. The protocol layer helps Jointer remain in compliance and update the whitelists to reflect potential KYC/AML changes.

In addition, the processor authorizes different holding periods or other regulatory limitations for wallets. Rules can be added or subtracted based on the nature of ever changing regulation.

**Example**

The whitelist is currently set to exclude people based on KYC/AML and accreditation checks.
The whitelist processor adds additional layers of restrictions such as the current restriction to exclude users from North Korea.