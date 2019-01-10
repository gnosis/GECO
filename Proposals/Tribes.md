## Project Overview

### Project name

[Tribes](https://tribes0x.com)

### Team members

Derek Alia - Fullstack Developer - https://www.linkedin.com/in/derekalia/

### What project are you building

Tribes is a platform for communities, similar to Reddit and Patreon. It incorporates elements from blockchain cryptocurrency such as DAOs, monetary incentives, and governance to enable engaged communities.

### Why did you decide to build it

Tribes was born from the need to create better collaboration and monetization tools for people who create content.

### How long will it take

4 months.

### How much funding are you requesting

42k EUR.

### How did you hear about the GECO

I first heard about it from Mareen Gläske’s Medium post, “Unveiling the Gnosis Ecosystem Fund”.

## Your Proposal

### Project description

Tribes is a platform consisting of tribes which are collections of people centered around topics. Each tribe on our platform is a Gnosis Safe DAO with added smart contracts for extra functionality, including marketplaces and governance. We’ve made it easy for users to visit Tribes and begin using the Safe without having prior experience interacting with the blockchain, no metamask required. We allow creators to build their own tribe that is structured around the needs of their community. Each tribe can have paid monthly subscription tiers for community members who want greater access. Tribe members can get paid by receiving votes on the content they post to the tribe. Subscriptions to the tribe come in the form of ERC721 tokens that are created from the tribe you subscribe to. Every month subscription funds are sent to the moderators of the tribe and members who posted content and received votes. Tribes incentivizes an ecosystem of reputation and quality driven content creation.

An example of a tribe might be a community around a DutchX with custom modules allowing them to monitor and affect their DAO all from the tribes platform.

The goal of this project is to increase dapp usability and scalability. One of the ways we will achieve this is by creating a UI for tribe developers to code custom modules that interface with the Gnosis Safe and making those easily exportable for use outside of Tribes.

Another feature is to extend the Safe execution to allow for DAO type elements such as weighted votes. The execTransaction method takes into account how many members approve an action. The action gets process based on the number of users and the threshold set on the safe.

I would like to extend/build a module, to take into account a user’s percentage stake in a tribe. Similar to a company with stock, actions are decided by how board members vote (yes/no) and their stock portion. Therefore to execute a transaction we would take into account the users percentage of ownership which needs to be stored in a specified format on-chain.

This would be a simple and useful approach to DAO governance until we develop more interesting governance structures like Futarchy and Liquid Democracy.

There are two approaches I see right now to achieve this goal using Safe. One is to create a tribes smart contract which contains an execute transaction function that takes into account tribe member stake, how they voted, and the amount of time to wait until closing the request. This smart contract would be the owner of the tribe Safe and would execute an on-chain approval described [here](https://gnosis-safe.readthedocs.io/en/latest/contracts/transactions.html#on-chain-approvals). Another way is to build a module that interfaces with the Module Manager with similar functionality to the function described above.

Lastly, open sourcing our Safe modules will not only help us but also other blockchain projects that require similar functionality for their Safe. Tribes is taking a hybrid approach to decentralization and we plan on decentralizing core aspects such as storage and governance. Designing Tribes with modularity in mind to reach decentralization is an important goal.

This project will help onboard the next wave of users into the crypto space by significantly lowering UX barriers and providing real value for communities with governance, monetization tools, NFT engagement, lower fees, and censorship-resistance. The modules we create for Tribes will benefit scaling dapps and promote usability for new and experienced users.

### Features

**Governance module** - Simple governance add/remove users and features from the tribe or safe. More complex features will be added later.

**Custody Solution** - A solution that allows us to onboard users with zero knowledge of crypto and to make transactions on their behalf, mainly the handling of signing transactions without storing private keys.

**Tribe contract** - Rewrite token contract to be more modular and customizable for each tribe. Create an interface for erc721 tokens with Gnosis Safe.

**UX/UI** - Redesign the flow from on-boarding to trading tokens. I’ve personally designed most of the site and would prefer if a designer would join and create mockups that I can implement. I also need to create animations for actions and transitions on the frontend.

**Subscriptions** - Allow users to subscribe to a tribe without needing to sign a payment transaction every month. Two potential options to handle this, one is with meta transactions using EIP1337, and the other is to do manual transactions on a shared Safe with the user.

**Security Audit** - Once the token contract is ready we can start the contract audit phase. We expect this to take longer because of the back and forth required between developers and auditors.

### Team description

Derek Alia - Fullstack and web3 development experience. The Largest project that I've worked on is Simplr.ai, a service that enables distributed customer service workers to make money answering questions.

### Timeline, Milestones and Deliverables

**Phase I - Twilight Sparkle**

1. Develop Gnosis Safe integrations
2. Build a custody solution
3. Start Tribe contract
4. Hire a designer to help with UX flow and UI elements

**Deliverables**

Tribes should be able to allow new users to create ethereum accounts, spin up a tribe, add functionality, remove functionality, and allow users to purchase access tokens, which unlocks content.

**Time and Price Estimate**

1 month
10k EUR

**Phase II - Fluttershy**

1. Start OTC integration
2. Build subscriptions solution
3. Start development on governance
4. Begin development for Metamask users
5. Implement UX/UI

**Deliverables**

Tribes users should be able to purchase Dai/Eth with OTC provider or use Metamask to create/join a tribe. Members should be able to vote within a tribe and that result should affect the tribe/mods on-chain. Users’ accounts should be charged automatically for their subscriptions.

**Time and Price Estimate**

1 month
10k EUR

**Phase III - Applejack**

1. Subscriptions test
2. Tribe token test
3. Governance test
4. Security Audit
5. Finish UX/UI

**Deliverables**

Subscriptions and governance should be tested in a variety of ways to ensure safety. Develop functionality to extend Safe execTransaction function that takes into account governance elements. Start audit as soon as possible to apply fixes during the last month. UX mockups should be completed and implemented.

**Time and Price Estimate**

1 month
14k EUR

**Phase IV - Rainbow Dash**

1. Testing
2. Implement changes from audit
3. Alpha test - On-board projects and communities

**Time and Price Estimate**

1 month
8k EUR

**Deliverables**

Implement feedback from security audit and begin on-boarding selected communities. Achieve 80% test coverage and all flows have been through multiple rounds of user testing.
