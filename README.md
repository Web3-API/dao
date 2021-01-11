# Web3API DAO
[![Generic badge](https://img.shields.io/badge/Wallet-Aragon-52EBFF.svg)](https://client.aragon.org/#/w3api) [![Generic badge](https://img.shields.io/badge/Consensus-Snapshot-f6ad32.svg)](https://snapshot.page/#/web3-api)  

The `Web3API` token holders, known collectively as the "DAO", are responsible for stewarding the Web3API ecosystem. The DAO controls the:
- Treasury
- Token minting
- DAO configuration
- ENS domain (web3api.eth)

In the future, it is anticipated that the DAO will also govern:
- Web3API repositories
- Web3Hub platform deployments
- DAO-verified APIs (hosted at web3api.eth subdomains)

## Join The DAO

Interested in getting involved?

1. Start out by joining our [Discord](https://discord.gg/Z5m88a5qWu) or reaching out to the point person for your area of interest:

| Domain| Points of Contact |  
|-|-|
| [Web3API Core Client](https://github.com/Web3-API/prototype) | [Jordan](https://t.me/dOrgJelli) |  
| [Web3API Standard](https://github.com/Web3-API/specification) | [Belma](https://t.me/MorriganIV), [Jordan](https://t.me/dOrgJelli) |  
| Web3Hub | [Andrew](https://t.me/cncrde) |  
| [Landing Page](https://github.com/Web3-API/landing-page) and [Branding](https://github.com/Web3-API/branding) | [Roberto](https://t.me/daoadvocate) |  
| [Twitter](https://twitter.com/web3api) and [Substack](https://web3api.substack.com/) | [Ingamar](https://t.me/Ingalandia) |
| Launch Partners | [Steff](https://t.me/SteffBrowne) |
| Tokenomics | [Phil](https://t.me/phil_h), [Ori](https://t.me/Ori) |

2. Submit a proposal on [snapshot](https://snapshot.page/#/web3-api) using our [template](./spending-proposals/000-TEMPLATE.md) and compensation guidelines (below).

3. If your proposal is accepted, add the details [here](./spending-proposals/) and make sure to update this with details as you progress (you are also encouraged to regularly share updates in community chats and calls).

4. Submit payment proposals on [Aragon](https://client.aragon.org/#/w3api) at the delivery milestones laid out in your proposal.*

### Compensation Guidelines

Here are some guidelines for making your spending proposals. These guidelines are just guidelines, as all final decisions are made by the DAO.

Choose an hourly rate commensurate with your level of relevant experience and desired weighting between USD and `W3API`. 

| Level | Years of Experience| Option 1 | Option 2  | Option 3 | Option 4 |
|-|-|-|-|-|-|
| Junior | 0-2| 0.05 `W3API`, $50 | 0.125 `W3API`, $35 | 0.225 `W3API`, $20 | 0.375 `W3API`, $0 |
| Intermediate | 2-4 | 0.06 `W3API`, $65 | 0.15 `W3API`, $50 | 0.27 `W3API`, $35 | 0.45 `W3API`, $0 |
| Senior | 4+ | 0.07 `W3API`, $80 | 0.175 `W3API`, $65 | 0.315 `W3API`, $50| 0.525 `W3API`, $0 |

We also suggest starting at 25% below your rate for a 4 week trial period.

\* *Please keep in mind that all final decisions must be approved by the DAO.*

## Token Distribution
> NOTE: Tokens are initially set to be non-transferable.

<img src="./bin/token-distribution.png" width="300px"/>

### Dev Mining

The DAO plans to mint no more than 12,000 tokens to incentivize builders and build the DAO treasury from Oct 1, 2020 through Dec 31, 2021. Below is a suggested schedule for the builder payouts, with a designated Treasury/Buffer beginning January 2021 to serve as a surplus resource for future usage (integration grants, partnerships, fundraising, insurance, liquidity, etc.).*

|  | Period | Builder Payout Ceiling | DAO Treasury/Buffer |
|-|-|-|-|
| 1 | Sep-2020 | 200 | |
| 2 | Oct-2020 | 200 | |
| 3 | Nov-2020 | 400 | |
| 4 | Dec-2020 | 400 | |
| 5 | Jan-2021 | 500 | 400 |
| 6 | Feb-2021 | 500 | 400 |
| 7 | Mar-2021 | 500 | 400 |
| 8 | Apr-2021 | 500 | 400 |
| 9 | May-2021 | 500 | 400 |
| 10 | Jun-2021 | 500 | 400 |
| 11 | Jul-2021 | 500 | 400 |
| 12 | Aug-2021 | 500 | 400 |
| 13 | Sep-2021 | 500 | 400 |
| 14 | Oct-2021 | 500 | 400 |
| 15 | Nov-2021 | 500 | 400 |
| 16 | Dec-2021 | 500 | 400 |
| | TOTAL | 7,200 | 4,800 |

\* *Please keep in mind that the DAO can decide to change these plans at any time*

### Pre-Seed Builders
At launch 4,000 `W3API` were minted to *Pre-Seed Builders* in proportion to work contributed before launch on October 1st (viewable [here](./token-allocations/pre-seed-builders.csv)).

### Pre-Seed Funders
4,000 `W3API` were minted to *Pre-Seed Funders*, enabling the DAO to raise $1M by the end of 2020. Tokens were priced in three batches (viewable [here](./token-allocations/pre-seed-funders.csv))

  | Batch | Supply | Price |
  |-|-|-|
  |~~*A*~~ (filled)|~~1,500 `W3API`~~|~~$200~~|
  |~~*B*~~ (filled)|~~1,500 `W3API`~~|~~$250~~|
  |~~*C*~~ (filled)|~~1,000 `W3API`~~|~~$325~~|

## DAO Configuration

Initial governance parameters are as follows:
| Parameter | Value | Description |
|-|-|-|
| *Minimum Approval* | 10% | Percentage of the total token supply that is required to vote “Yes” on a proposal before it can be approved. |
| *Support* | 60% | Relative percentage of tokens that are required to vote “Yes” for a proposal to be approved. |
| *Vote Duration* | 7 days| Maximum length of time that the vote will be open for participation. |

The DAO uses the following Aragon apps:
| App | Address | Description |
|-|-|-|
| *[Voting](https://help.aragon.org/article/19-voting)* | 0x5f78d0668ba666b4ed9674b313419d9db6cd48a6 | Used to create and participate in votes. Votes can be linked to an action, such as minting `W3API` or transferring funds, or be purely informative. |
| *[Finance](https://help.aragon.org/article/20-finance)* | 0xc19a9f41df38e0f01f809d257d6c71f892adaaff | Manages the organization's financial assets, including ETH and ERC20s. |
| *[Tokens](https://help.aragon.org/article/18-tokens)* | 0x8baa4cd6bf2a01e96e421c18b0231ce7791ed869 | Manages the supply and distribution of `W3API`. |
| *[Token Request](https://github.com/1Hive/token-request-app/blob/master/docs/user-guide.md)* | 0x9bb4ea752a3096104c7765ad318b0f9cabaaf95f | Mints `W3API` in exchange for payment.|
| *[Agent](https://help.aragon.org/article/37-agent)* | 0x8fe59d8fb5ffd3509e5cb3d386be8bdb2d363662 | Enables the organization to interact directly with any other smart contract on Ethereum. For example, setting an ENS resolver. |

See the full configuration [here](https://client.aragon.org/#/w3api/permissions/).

\* *Please keep in mind that the DAO can decide to change its configuration at any time*

## Legal

Holders of `W3API` do not constitute any sort of partnership or joint venture, only the right to participate in the governance of the DAO. Further, becoming a Builder does not constitute any sort of partnership, joint venture, principal-agent relationship, or an employer-employee relationship. 
