# DAO Migration

| Funds Requested | Time Period | Estimated Effort 
|-|-|-|
| Gas Reimbursement | June 1 | 6 hrs |

## Summary

This proposal is to migrate our DAO from Aragon to Gnosis Safe + Snapshot. This will also include a redeployment of the token contract that migrates all existing balances and changes the token ticker to `WRAP-IOU` and name to `PolyWrap IOU Token` as part of the ongoing rebrand.

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

The main drawback of this approach is that execution is no longer autonomous as is the case with Aragon, since the multisig signers must be trusted to act in accordance with Snapshot proposals. To mitigate this risk in the near-term, we will use a representative sample of the top 2/3rds of token holders as signers, updated quarterly based on token holdings.

Furthermore, migrating to Safe + Snapshot positions us to be an early adopter of the recently released SafeSnap product, which utilizes the Reality.eth oracle service to guaruntee that the Safe can only execute transactions approved by Snapshot proposals. We will continue to interface with the SafeSnap team to evaluate when this solution is ready for us to migrate to.

### Migration Plan

1. Deploy 6-of-12 Gnosis Safe with the following owners:

    | Address | Current Supply % | Votes |
    |-|-|-|
    | 0xb1b7586656116d546033e3baff69bfcd6592225e | 24.37% | 3 (2 proxies) |
    | 0x639749b7b08aee65039c21d8a411103c6cebebf0 | 10.41% | 2 (1 proxy) |
    | 0xf2d89aed137edab8be23584b43621024869e6d39 | 7.39% | 1 |
    | 0x37341cbb14c5f128a70b149726ad8b2ce6f4c793 | 6.85% | 1 |
    | 0x32087947f4ea79c3e17f84bc2d0e5212fdeca668 | 4.93% | 1 |
    | 0xef7cfd3a5a1a9ddd3f4582f14b9a98b3e86eded1 | 4.06% | 1 |
    | 0xd8879be0032092eb5e610d5a2ab64e56ae010348 | 3.09% | 1 |
    | 0xbd9f96663e07a83ff18915c9074d9dc04d8e64c9 | 3.05% | 1 |
    | 0x58b753f0c417494226af608b63e80028255cbc64 | 2.87% | 1 |

2. Deploy new token contract
    - Deploy from the Safe with the Safe set as the owner with minting permissions
    - Seed the distribution with snapshot of [`W3API` balances](https://etherscan.io/token/0x9F59E5Ed123C10D57E92629612511b14628D2799)
    - Keep transferrability turned off but changeable by owner

3. Create proposals on Aragon to transfer all funds to the Safe 

4. Setup snapshot page with new token
