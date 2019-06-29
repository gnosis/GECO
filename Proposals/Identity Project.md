# Proposal Outline: Identity

## Project Overview

### Project name

> Identity

### Team members

> Dennison Bertram - Developer and Developer Advocate at OpenZepelin.

> Seth Feibus - Developer at dOrg, Relevant.community. Creator of Statesauce - a Javascript Web3 state management library. Founder at NIfty Supply

### What project are you building?

> An Identity contract on Ethereum that can represent users as a first-class citizen in Ethereum.
> ERC725 compliant, MetaTransaction enabled, and Gnosis Multi-Sig for Social Recovery, 2FA, transferable accounts, and fine grain permission controls.
> Identity can execute arbitrary function calls, and both create and create2 contracts. An Identity also stores metadata allowing the user- be it organizations,
> individuals, DAO's or otherwise, to keep a public (or encrypted) record of documentation related to the identity.

### Why did you decide to build it?

> I have been working on two projects: A Doctor Dao where patients can request Vaccination records from DAO doctors, and a Digital art Archival tool for artists.
> In the process of building these two projects, I realized that there was an overlapping base component that was missing: Identity. Both the Doctor Dao and the
> artist project needed a way to represent an Identity on the blockchain with associated MetaData. In the case of the Doctor Dao- doctors need to supply their public credentials stored in metadata, whereas the patients can link themselves through family in encrypted metadata and medical notes for vaccinations.
> In the case of Artists, a singular contract that could act as the authoritative source of an artists archive needed the ability to create new token lineages that represent their art, along with Metadata to describe themselves and create a catalog.
> For both these projects, I need an Identity. Something easy to use (MetaTxns for onboarding issues), but also something forgiving- Gnosis multisig for Social Recovery
> and flexible but secure permission model.

### How is Gnosis Multi Sig relevant to your project?

> To improve upon the current public-private key pair system for signing transactions on ethereum, we need to create a second layer permissions system.
> This is only possible using Gnosis MultiSig. Features such as social recovery, portable identities, two-factor authentication are all features that are built using Gnosis MultiSig contracts.
> It is a critical component.

### How long will it take?

> The project I have broken down into phases. Each phase will incrementally improve the usability and developer experience of the Identity platform.
> I estimate 1 quarter for each phase, with a total of 4 quarters to deliver a polished, production level product accessible to the average front-end _developer_.
> Note that my target is not limited to _web3_ developers. My goal is to create something simple and open for developers.

### How much funding are you requesting?

> Each phase has a different estimated requirement for funding. I have already finished a working proof-of-concept so the first phase the funding I am requesting is lower
> than the others which have yet to be started.
> Phase 1: Completion of the base Solidity Code + testing: $10,000
Phase 2: Creation of a Javascript library part 1: A javascript API for interacting with the Identity smart contract code. $17,000
> Phase 3: Stretch Goal: Creation of a Javascript library part 2: Gasless, keypair-less usage for web2 style onboarding: $15,000
Phase 4: Stretch Goal: Documentation and Tutorials: $6,000
> Phase 5: Stretch Goal: Auditing: Unsure, the goal is a community project. So a community audit should be requested.

### How did you hear about GECO

> Twitter, and Seth, who works on the Continuously Funded DAO Project, supported by GECO.

# Proposal

## Project description

> Identity is a first-class citizen as a smart contract. It builds upon the draft ERC725 standard and expands it to create an Identity that can practically represent a user or
> organization on the blockchain- without needing them to hold Eth or use MetaMask.
> Onboarding regular users to Ethereum requires giving users an experience that does not require eth or MetaMask to securely interact with. There are many use
> cases for ethereum that largely do not revolve around finance, but are underserved by the current community tools. Identity is to be an open source tool that is
> platform agnostic, any developer can build upon it free of charge. Identity is a _building_ block for more inclusive, low-friction blockchain backed applications.
> Identity seeks to build a free, open source building block for developers. Identity is not the business model in and of itself. It is community software so everyone
> can build more powerful, more inclusive, applications.

## Features

> Identity is built using ZeppelinOS. This allows for iterative development, modularity via EVM packages of on-chain code libraries, and optional upgradability of contracts.

> The smart contracts are written using solidity. The Javascript library is written using Nodejs.

> Identity is compatible with the ERC725 proposal for Identity contracts.

> MetaTransactions are powered by the Gas Stations Network which will be released soon by Zeppelin, TabooKey and the Gas Stations Network Alliance.

> Social Recovery, ownership portability, and personal account recovery are provided by Gnosis multisig. The javascript library will give an easy way to use these functions.

> OpenZeppelin Roles are used to guard permissions.

> MetaData is stored in contract with a caching feature to minimize API calls.

> Javascript library will utilize IPFS/OrbitDB or Swarm for storage of metadata and encryption.

## Team description

Dennison Bertram - Developer Advocate at OpenZeppelin.

https://github.com/crazyrabbitLTC

> Created the first Bitcoin exchange in the Czech Republic called BuyBTC.cz in 2012.
> As developer advocate, runs frequently workshops on building DApps and creates numerous DApp development tutorials in his role as Developer Advocate.

> Master of Ceremonies of ETH New York 2019, and prize winner at the ETH Buenos Aires hackathon (Status and OpenZeppelin Prize), MakerDao prize winner at Status IM Hackathon during Devcon 4, and WindingTree during Devcon 4 hackathon among others.

> Member of CryptoNYC.

Seth Feibus - Freelance Developer, Founder of Nifty Supply.

https://github.com/sethfork

> Contract developer at Relevant.community and dOrg.tech, where he works on several Ethereum projects including a Continuous Funding scheme for the dxDAO (Supported by GECO), and an Identity DAO project.

> Creator of Statesauce, a Javascript framework for developing web3-enabled applications.
> https://github.com/statesauce/redux-saga-web3

> Member of CryptoNYC and winner of 2 prizes at ETH Denver 2019 Hackathon.

Both team members are NYC based, share co-working space at CryptoNYC and have collaborated previously.

# Timeline, Milestones, and Deliverables

## **Phase I**: Completion of the base Solidity Code + testing

In this phase, the working code of the first version is completed. Currently, the code is at Alpha status and is functional with a limited set of passing tests for some of the more
challenging features (Create2 contract creation, arbitrary code execution)
**Deliverables** _What features will be implemented_

A working v1 beta-version of the code. All base functionality completed:

Modularity: Functionality is implemented via ZeppelinOS EVM packages. Each group of functionality is isolated in an individual EVM package to create a composable application.

Draft ERC725 functionality: (following: https://github.com/ethereum/EIPs/issues/725)

MetaTransaction support: Incorporation of Gas Stations Network

Gnosis MultiSig integration: Support for Social Recovery and various recovery mechanisms.

**Time and Price Estimate:**  
\$10,000
4-6 Weeks.

> Most of the Alpha code is completed and working.
> There is substantial refactoring to do, but much of the code builds upon code already developed by the community and composes it to a larger organism.
> The majority of the work here is refactoring, breaking the solidity code into EVM package modules and designing a more complete set of tests.

---

## **Phase II:** Creation of a Javascript library part 1: _A javascript API for interacting with the Identity smart contract code_.

In this phase, a nodejs library is built to simplify the process of interacting with Identity. Currently, things like executing arbitrary code via smart contract are cumbersome
for most developers to implement. Creating and managing `create2/create` contract creation requires a number of utility functions and various steps to do, which make it
harder to work with.

**Deliverables** _What features will be implemented_
Javascript library for creating and interacting with Identities.

1. Creation of Identities
2. Creation/Execution of arbitrary code via Identities
3. Creation, updating metadata for Identities.
4. Social Recovery and Recovery patterns for identities.

The goal is to make all the various tasks that could be completed with an Identity something that can be executed as a method on a created `Identity` instance.
IE:

```
const id = new Identity({config});
id.execute();
id.createRecovery();
id.sendEth();
etc...
```

**Time and Price Estimate:**
\$17,000
8-10 weeks

> This is the most complicated part of the project. We will need to spec out the design for the library and its requirements, then build and test it.
> The v1 of the library will encapsulate the most common tasks that a developer using Identity would run into. The important points are simplifying the usages of Gnosis Multi-sig for recovery processes and simplifying executing arbitrary functions on-chain.
> These are the highest points of developer friction in the process.

---

## **Phase III:** Stretch Goal 1: Creation of a Javascript library part 2: _Gasless, keypair-less usage for web2 style onboarding_

IPFS/SWARM integration for storage and retrieval of Metadata.

Metadata Caching for reducing API usage.

The effectiveness and usability of MetaTransactions depend on developers being able to effectively keep track of Ephemeral use keypairs. This phase will create tools to help developers do this in a simple, web2 style manner using technologies web2 developers are already familiar with. This should not be the
core of any effective decentralized system but is important for the onboarding process.

I understand this does not feel "totally crypto" but it's very necessary for practical onboarding of developers and users. Any DApp can require that a user,
after 5 transactions (for example) must set up a new MetaMask and transfer full control to the user's responsibility. However, we lose users by requiring
MetaMask, 12 words, KYC for ETH, etc... at the very start.

**Deliverables**

Javascript front end Library for generating and managing Ephermeral Keypairs
Metadata Caching with IPFS and OrbitDB
Demo express server for encrypting recovery keypairs
Demo OATH integration for recovery keypairs.

**Time and Price Estimate:**
\$15,000
8-10 weeks.

---

## **Phase IV:** Stretch Goal 2: Documentation and Tutorials

A project is only as useful as one can communicate it. As a Developer Advocate, I know first hand the importance of sharing educational materials: Tutorials, guides, documentation.
While documentation is an important part of each phase, focusing on the complete project requires its own phase to create a unified body of documentation.
This phase of the project is intended to clearly illustrate in a simple to follow tutorials and guides how to use Identity, how to integrate it into a project, and how to access all the features offered by it.

Documentation: Developers need an API reference to understand the ins and outs of a project. Everything needs to be clearly understandable, clearly written. A reference for when working with Identity, the contracts and the Javascript library.

**Deliverables**

A website containing tutorials, examples, documentation and sample code.

**Time and Price Estimate:**
\$6,000
4-6 weeks.

---

## **Phase V:** Auditing

This is the final stretch goal, and I feel is beyond the scope of the Gnosis ecosystem grant. We will need auditing services, but as a community project, this must be something that the community feels is important and is either willing to help out with or fund. I am not including it as a grant request at this time from Gnosis. Depending on the reception and
success of Identity, I can propose this in the future for a grant.

**Cost Estimate:**
This would be performed by a reputable auditing company, the cost estimate would depend on their estimates.
