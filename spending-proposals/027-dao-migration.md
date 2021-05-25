# DAO Migration

| Funds Requested | Time Period | Estimated Effort 
|-|-|-|
| Gas Reimbursement | June 1 | 4 hrs |

## Summary

This proposal is to migrate our DAO from Aragon to Gnosis Safe + Snapshot. This will also include a redeployment of the token contract that migrates all existing balances and changes the token ticker to `WRAP` and name to `PolyWrap Token` as part of the ongoing rebrand.

## Detailed Deliverables

### Justification

There are several problems with the current Aragon setup:
- Creating and voting on proposals is prohibitively expensive
- Can only send one token type to one address at a time, which results in worse UX and additional cost
- Difficult to perform complex operations such as treasury management, ENS, liquidity provision, airdrops, streaming payments, etc.

Here is how the Safe + Snapshot setup would mitigate these problems:
- Creating proposals and voting on Snapshot is free
- Safe's Transaction Builder app makes it easier to chain together multiple transactions, such as a batched payment, into a single atomic action
- Safe allows for generic contract interaction and supports a growing suite of easy-to-use apps like Superfluid, 1inch, ENS, and Yearn

The main drawback of this approach is that execution is no longer autonomous as is the case with Aragon, since the multisig signers must be trusted to act in accordance with Snapshot proposals. We believe that this risk can be mitigated in the near-term by having a representative sample of the top 51% of token holders selected as signers.

Furthermore, migrating to Safe + Snapshot positions us to be an early adopter of the recently released SafeSnap product, which utilizes the Reality.eth oracle service to guaruntee that the Safe can only execute transactions approved by Snapshot proposals. We will continue to interface with the SafeSnap team to evaluate when this solution is ready for us to migrate to.

### Migration Plan

1. Deploy 4-of-7 Gnosis Safe with the following owners:
  - 0x...
  - 0x...
  - 0x...
  - 0x...
  - 0x...
  - 0x...
  - 0x...
2. Deploy new token contract
  - Deploy from the Safe with the Safe set as the owner with minting permissions
  - Seed the distribution with existing balances plus pending approved token rewards (TODO - attach table of existing token holders plus new issuance to this proposal)
  - Keep transferrability turned off but changeable by owners
3. Create proposals on Aragon to transfer all funds to the Safe 
4. Create snapshot page with new token (is there a way to convert the current snapshot page to a new token address?)
