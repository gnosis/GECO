# DutchX Subgraph

## Project Overview

The project being proposed in this document is a supplementary data management solution for the DutchX protocol built using [The Graph](https://thegraph.com/).

This project was conceived of at the recent [ETHDenver Buidlathon](https://www.ethdenver.com/). Both Gnosis and the The Graph were sponsoring awards for anyone that used their solutions in an entry. Having some experience using the DutchX, I knew that historical data storage and access is something that could be improved upon in the DutchX and saw that The Graph offered a good solution.

**POC**: [Hackathon Entry](https://github.com/g-r-a-n-t/dutchx-subgraph) (winner of both competitions mentioned)

**Time**: ~2 months

**Funding**: $15,500

**Referral Source**: Mareen Gläske

**Team Members**:
- Grant Wuerker
  - LinkedIn: https://www.linkedin.com/in/grant-wuerker-6a687284/
  - Github: https://github.com/g-r-a-n-t

## Proposal

The Graph is a general purpose data persistence solution for Ethereum. It uses events emitted by the Ethereum network to update entities in its database and allows for the retrieval of these entities using [GraphQL](https://graphql.org/). Developers are able to create what's known as a "subgraph" to integrate their projects with the platform.

The DutchX, being a protocol developed entirely using smart contracts, stands to benefit from the Graph significantly, as it would make the storage of historic information cost-efficient and flexible and the retrieval of information simple.

By creating a subgraph, developers are able to separate the storage of historic data from data that is required for smart contract execution. This design is somewhat analogous to traditional application design where long term storage is delegated from memory to disk due to physical limitations. In the current Ethereum system, long term storage on the blockchain is free after initial costs. However, it is likely that mechanisms will be introduced in the future that disincentivize this behavior [[x]](https://ethresear.ch/tags/storage-fee-rent). If this is the case, it would make sense from an economic perspective to lean out smart contract storage and leverage a specialized storage tool for data that is not functionally necessary. The specialized storage tool in this case is The Graph.

There are also considerations relating to iterability. Since the management of entities is handled off-chain, it is possible to make changes to the subgraph frequently. In comparison to the DutchX API, where data is pulled directly from smart contracts, adding new endpoints could be hindered by limitations in the contracts. A subgraph does not have this issue since it does not source data directly from smart contracts. As long as you can find an event that is relevant to the entity, you can keep it up-to-date.

In terms of developer appeal, a subgraph has some charms. To name a few: GraphQL is a powerful open-source language built for contemporary applications. It is easy to learn and can be used to perform complex tasks. Being able to perform queries on the DutchX using GraphQL would be very cool. In addition to this, The Graph has built an explorer, so if developers want to learn how to use the DutchX subgraph without configuring their environment, they can just go to this [page](https://thegraph.com/explorer/subgraph/g-r-a-n-t/dutchx) and try it out. Both of these things would make the DutchX subgraph appealing to anyone hoping to build on the platform. There is a wide range dapps people could use this subgraph for, but some examples include: Exchange interfaces, analytical software, and trading bots.

### Features

Below is a table showing which events currently exist in the DutchX and the entities that they could **potentially** map to. Note that there would not be any changes made to the DutchX contracts themselves; the subgraph would be implemented as a standalone component that uses existing events.

contract       | event                 | entities                       | phase
-------------- | --------------------- | -------------------------------| ---
DutchExchange  | NewDeposit            | Balances, Deposits             | I
DutchExchange  | NewWithdrawal         | Balances, Withdrawals          | I
DutchExchange  | NewSellOrder          | Balances, Auctions, SellOrders | I
DutchExchange  | NewBuyOrder           | Balances, Auctions, BuyOrders  | I
DutchExchange  | NewSellerFundsClaim   | Balances, SellerFundsClaims    | I
DutchExchange  | NewBuyerFundsClaim    | Balances, BuyerFundsClaims     | I
DutchExchange  | NewTokenPair          | Markets                        | I
DutchExchange  | NewAuctionScheduled   | Auctions                       | I
DutchExchange  | NewAuctionCleared     | Auctions                       | I
DutchExchange  | Fee                   | Fees                           | I
DxUpgrade      | NewMasterCopyProposal | MasterCopyProposals            | II
EthOracle      | NewOracleProposal     | OracleProposals                | II
TokenWhitelist | Approval              | WhitelistedTokens              | II
DsAuth         | LogSetAuthority       | LogSetAuthority                | II
DsAuth         | LogSetOwner           | LogSetOwner                    | II
DsNote         | LogNote               | LogNotes                       | II

*The entities listed above could be subject to change.*

### Team

Grant Wuerker, the sole developer on the proposed project, has been working in the field of computer science for ~6 years. He has experience working in academic research, system administration, and software engineering as well as experience working on the Gnosis Safe via Gitcoin. His interest in decentralized systems stems from a belief that this technology will lead to a more fair and transparent world. Any opportunities to contribute to the ecosystem in a sustainable way are met with excitement.

### Timeline, Milestones and Deliverables

The development of this project would be broken up into four phases. Two of which would be coding the project, one is is for documentation, and another is for making changes that come out of a review from the DutchX team.

---

**Phase I**: `DutchExchange.sol` entities and listeners

**Deliverables**: All entities and listeners for the `DutchExchange.sol` contract are implemented. Each functional unit of code would have sufficient test coverage.

**Time and Price Estimate**	3 weeks; $6,500

----

**Phase II**: Remaining entities and listeners

**Deliverables**: All entities and listeners for the remaining contracts are created. Each functional unit of code would have sufficient test coverage.

**Time and Price Estimate**	1 week; $2,250

---

**Phase III**: Documentation

**Deliverables**: Thorough documentation around technical implementation and usage.

**Time and Price Estimate**: 2 weeks; $4,500

---

**Phase IV**: Changes based on review

**Deliverables**: Any changes that come out of a review from the DutchX team.

**Time and Price Estimate**: 1-3 weeks (dependent on availability); $2,250

