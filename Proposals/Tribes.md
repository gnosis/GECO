## Project Overview

### Project name

[Tribes](https://tribes0x.com)

### Team members

Derek Alia - Fullstack Developer - https://www.linkedin.com/in/derekalia/

### What project are you building

Tribes is a platform for online communities, similar to Reddit and Patreon. It incorporates elements from blockchain cryptocurrency such as DAOs, monetary incentives, and governance to enable engaged communities.

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

## Project Overview

### Project name

[Tribes](https://tribes0x.com)

### Team members

Derek Alia - Fullstack Developer - https://www.linkedin.com/in/derekalia/

### What project are you building

Tribes is a platform for online communities, similar to Reddit and Patreon. It incorporates elements from blockchain cryptocurrency such as DAOs, monetary incentives, and governance to enable engaged communities.

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

Tribes is a platform where people drawn to a specific topic come together to form an online community, or "tribe". Each tribe on our platform is a Gnosis Safe DAO with additional smart contracts for extra functionality, including marketplaces and governance. We’ve made it easy for users to visit Tribes and begin using the Gnosis Safe contract without having prior experience interacting with the blockchain--no Metamask or other extensions are required. We allow creators to start a tribe that is structured around the needs of their community. Each tribe can have paid monthly subscription tiers for community members who want greater access. Tribe members can get paid by receiving votes on the content they post to the tribe. Subscriptions to the tribe come in the form of ERC721 tokens that are created when a user subscribes to a tribe. Every month subscription funds are sent to the moderators of the tribe and members who posted content and received votes. Tribes incentivizes an ecosystem of reputation and quality driven content creation.

An example of a tribe might be a community around a DutchX with custom modules allowing them to monitor and affect their DAO all from the Tribes platform.

An important goal of Tribes is to increase dapp usability and scalability. One of the ways we will achieve this is by creating a UI for tribes to add custom modules that interface with the Gnosis Safe contract and make the modules easily exportable for use outside of the Tribes platform.

Another feature is to extend the Gnosis Safe to allow for DAO type elements such as weighted votes. Currently, the Gnosis Safe executes by taking into account how many members approve an action. The action gets processed based on the number of users and the Safe's threshold.

I plan to build a module that takes into account a user’s stake in a tribe. An action will be executed depending on how members vote (yes/no) and the weight of each member's vote will depend on his or her stake in the tribe. Prior to deploying this module, members will agree on a voting threshold that must be met for approving an action. This would be a simple and useful approach to DAO governance until we develop more interesting governance structures like Futarchy and Liquid Democracy.

Open sourcing Tribes' governance module will help other blockchain projects that require similar functionality for their Gnosis Safe. Tribes takes a hybrid approach to decentralization and I plan on decentralizing core aspects such as storage and governance. Designing Tribes with modularity in mind to reach decentralization is an important goal.

This project will help onboard the next wave of users into the crypto space by significantly lowering UX barriers and providing real value for communities with governance, monetization tools, NFT engagement, lower fees, and censorship-resistance. The modules created for Tribes will benefit scaling dapps and promote usability for new and experienced users.

### Features

**Governance module** - Module to change Gnosis Safe contract execution based on users ownership percentage in the tribe and the direction of their vote. The module will set a time duration for each vote. The UI for interacting with this module will be built out as an NPM package for other projects to use.

**Safe Module UI** - A ReactJs UI for adding and removing modules to a Gnosis Safe.

**Custody solution** - A solution that allows Tribes to onboard users with zero knowledge of crypto and to make transactions on their behalf, mainly the handling of signing transactions without storing private keys.

**Tribe contract** - Each tribe uses this contract it's a modular and customizable token contract keeping track of subscribers, Gnosis Safe, member stake, and subscription tiers.

**Subscriptions** - Users can subscribe to a tribe without needing to sign a payment transaction every month. Two potential options to handle this, one is with meta transactions using EIP1337, and the other is to do manual transactions on a shared Safe with the user.

**Security audit** - Once the token contract is ready Tribes can start the contract audit phase. I expect this to take longer because of the back and forth required between developers and auditors.

**UX/UI** - Tribes will develop fundamental UX flows from onboarding to trading tokens. I’ve personally designed most of the site and would prefer if a designer would join and create mockups that I can implement. I also need to create animations for actions and transitions on the frontend.

### Team description

Derek Alia - Fullstack and web3 development experience. The Largest project that I've worked on is Simplr.ai, a service that enables distributed customer service workers to make money answering questions.

### Timeline, Milestones and Deliverables

**Phase I - Twilight Sparkle**

1. Build a custody solution
2. Develop tribe contract
3. Develop Gnosis Safe contract integrations
4. Hire a designer to help with UX flow and UI elements

**Deliverables**

Tribes will create an ethereum account on behalf of the user if they do not already have Metamask installed. The custody solution allows users to interact with the Gnosis Safe contract and the ethereum blockchain all within the browser and without third-party plugins. For example, users using Safari browser on mobile will be able to interact with the Gnosis safe securely. We can do this by using a two-factor authentication approach as described in the [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki). This is an important step because it lowers the barrier for people who are new to the blockchain space and want to use its services. The only requirement for the user to sign transactions is to remember their password.

Once the user has the ability to sign transactions we can enable them to start a tribe or subscribe. To start a tribe the user inputs all the requirements and the type of community to launch, such as a single creator, multi-creator, subscription tiers, allocation of funds, and governance style. The tribe contract will take this information into account and setup a Gnosis Safe contract with the required modules. The Gnosis Safe contract will also be responsible for sending funds to creators on a monthly basis.

**Time and Price Estimate**

1 month
10k EUR

**Phase II - Fluttershy**

1. Start fiat to crypto integration
2. Build subscriptions solution
3. Development flow for Metamask users
4. Start development on governance module
5. Implement UX/UI

**Deliverables**

A path for users to purchase ETH after going through a KYC process. We plan on using a fiat to crypto provider to help us with this approach but it is necessary to make sure this flow is very clear and easy to follow. This is an important step to allow users to pay gas to send transactions. The two most common transactions will be setting up a tribe and subscribing to a tribe. For the subscription solution, we intend to use the [ERC948](https://github.com/ethereum/EIPs/pull/1337) contract as the first approach. Ultimately this will allow creators to receive funds every month without the user having to sign each month.

For users who are uncomfortable with using a two-factor custody process for signing transactions, we will enable a path for them to use Metamask instead. Using Metamsk implies that the user probably has ETH and does not need to go through our fiat to crypto process. Creating a different signing pipeline will be created to enable this.

A working version of the governance module that interfaces will the Safe of a tribe. When tribe members request to change a setting this starts the governance process of taking in votes, checking the users' stake in the tribe and the direction of the vote. The decision of the vote can change settings on the tribe's Gnosis Safe or tribe contract, modifying users stake, adding/removing a user, and adding/removing a module.

New UI/UX mockups should be 30-50% finished. Development on those mockups into code will have started.

**Time and Price Estimate**

1 month
10k EUR

**Phase III - Applejack**

1. Subscriptions test
2. Develop Safe Module Manager UI
3. Tribe token test
4. Governance test
5. Security Audit
6. Finish UX/UI

**Deliverables**

Subscriptions and governance will be tested in a variety of ways to ensure safety. A UI for pausing and canceling subscriptions to allow the user full control of their subscriptions.

Basic UI for users to add and remove modules to the Safe. This feature will be integrated into each tribe to manage module functionality.

Once this is complete we can start the audit as soon as possible to apply fixes during the last month. UX mockups should be completed and implemented.

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

Implement feedback from security audit and begin onboarding selected communities. Achieve 80% test coverage and confirm all flows have been through multiple rounds of user testing.

**Other**

_Governance_
Tribes is creating a module for the Gnosis Safe which is a smart contract to enable governance. It will take into account each users percentage of ownership of the organization. On deployment, the user will set a threshold of how much percent is needed to pass a vote and the duration for each vote.

An example would be three people start a tribe/organization and set the threshold to 51 and the duration to 3 days. The ownership breakdown would look like the following:
Bob - 50%
Jill - 30%
Zane - 20%

At this point, Jill and Zane can’t pass a vote without Bob. To pass a vote they need at least 51%. As they grow they decide to add three more people (Tom, Sarah, Marc) to the project. The new breakdown is:
Bob - 45%
Jill - 27%
Zane - 19%
Sarah - 5%
Tom - 3%
Marc - 2%

Now there are more combinations to pass requests through the organization as it grows with new members. As standard, the Gnosis Safe contract execution function uses a threshold that looks at the number of approvals by members of the Gnosis Safe. While in most cases this works well, but if you have a growing organization with people coming in and out, using weighted votes gives more control to larger stakeholders before giving up so much control to new members. This is an example of how the governance module would function and why its needed going forward.

_Safe Module Manager UI_
Tribes will be creating a common interface for adding/removing new modules to the Gnosis Safe contract and developing this into a ReactJS NPM for other projects to use.

An example of this might be if a Gnosis Safe module is declared on Github a user would point to that URL and NPM would pull the description, contract code, and current version of that module. Then users would vote in order to have the package added to their Gnosis Safe modules.
  
_Adoption_
All tribes and potentially each user is a Gnosis Safe contract, we are pushing the adoption of Gnosis Safe DAOs. For perspective there are currently over 1 million subreddits on reddit.com, even 1% of that is a huge amount of Safe Contracts that we are hoping to create

_Reducing barriers_
I mention Metamask because most users interact with dapps by using Metamask. We are allowing users to use Metamask or other browser extensions to interact with our platform, but it is not a requirement. Our goal is to allow totally new users into the ecosystem and this is why I mention the custody solution, which is a system to generate a wallet for users who don't have one. With this method, users can interact with the blockchain and later on move to a more trustless system like the Gnosis Safe browser extension or Metamask.
