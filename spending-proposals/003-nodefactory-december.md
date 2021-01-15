# NodeFactory's services for December

| Funds Requested | Time Period | Estimated Effort |
|-|-|-|
| $8,000 + 103.2 `W3API` | Dec 1 - Dec 31, 2020 | 160 hours |

*Note that timeline is an estimate for the deliverables listed below.*

## Summary

NodeFactory proposes creating a first draft of technical specification, creating WASM interface definitions and improving the development cycle using Github actions CI.


## Deliverables

1. [Technical specification document (1st Draft Complete)](https://github.com/Web3-API/specification)
    * Some open PRs remain, as they're being iterated on.
    * All fundamental components of the architecture have been documented.
2. Setup CI on the [repository](https://github.com/Web3-API/prototype) that would run tests, check types and create build on pull requests and master push.
    * Done on both `master` and `prealpha-dev` branches
    * Only lint fixes are [pending PR](https://github.com/Web3-API/prototype/pull/90)  
3. [Create Web3 WASM interface definitions using Witx](https://github.com/Web3-API/prototype/issues/5)
    * Witx files for WASM interfaces (imports from host and exports from WASM) with generated Markdown files and generation instructions, pending review
    * CI integration that makes sure Markdown files are up to date


## Fund Distribution
All stable coins and W3API tokens should be send to: NodeFactory's address @ `nodefactory.eth` - `0xbD9f96663E07a83ff18915c9074d9dc04d8E64c9`.

| Name | W3API | Address |
|-|-|-|
| [NodeFactory](https://nodefactory.io/) | 16 | 0xbD9f96663E07a83ff18915c9074d9dc04d8E64c9 |  

## About us
NodeFactory is a blockchain research and development company based in Zagreb, Croatia. For the last 3 years, we are successfully providing services such as dApp development, infrastructure and tooling. More information about us and our work can be found on [nodefactory.io](https://nodefactory.io/) and [our portfolio](https://nodefactory.io/NodeFactory_portfolio_v5.pdf).

Belma Gutlic will be the point of contact for this work:
- https://github.com/morrigan  
- @morrigan88 (Keybase)
- @MorriganIV (Telegram)
