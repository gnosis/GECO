## Project Overview

### Project name

Orca Protocol

![image (2)](https://user-images.githubusercontent.com/44700178/110375463-ffddce80-801f-11eb-9f1b-81dcc940bbe3.png)


### What project are you building?

The team at Sonar Labs is building Orca Protocol: a lightweight community minting and management platform on Ethereum powered by Gnosis Safe. 

Orca Protocol empowers on chain communities to create, shape, and act in ways according to their values. The needs and shapes of these organizations vary dramatically and existing DAO frameworks lack the adequate systems or flexibility to accommodate the range of use cases. 

The Orca Protocol is an open source platform for individuals to pool their resources to pursuit a common endeavor by creating PODs, lightweight governance wrappers created around a Gnosis Safe. 

Once individuals join a POD they receive an NFT membership token to that POD. Members may propose Actions (arbitrary transactions) that are relayed through the Gnosis Safe. Additionally Members may vote on internal rules, such as membership requirements and voting schemes. Pods can also delegate voting power to one another allowing them to be arranged into organization hierarchies. 
Within the Orca Protocol Actions and Rules are designed as arbitrary transactions, meaning that PODs can be seamlessly integrate any application. We are looking forward to building out a large extensions library to make governance a totally seamless experience.

### Team members

![TeamOrca](https://user-images.githubusercontent.com/44700178/109559870-3c05b200-7aa9-11eb-8fec-04a0285f6a66.png)

**Julia Rosenberg, Product Lead** - [LinkedIn](https://www.linkedin.com/in/julia-rosenberg/) / [Twitter](https://twitter.com/Julia_R0senberg) 

**John Sterlacci, Head Engineer -** [LinkedIn](https://www.linkedin.com/in/john-sterlacci-28804594/) / [Twitter](https://twitter.com/JohnSterlacci) / [GitHub](https://github.com/jtlacci) 

**Steven Valeri, Blockchain Engineer -** [LinkedIn](https://www.linkedin.com/in/steven-valeri-69a64349/) / [Github](https://github.com/stevenvaleri) 

**Will Kim, Blockchain Engineer -** [LinkedIn](https://www.linkedin.com/in/william-kim-378316105/) / [Github](https://github.com/willKim19) 

**Daniel Thompson, Front End Engineer -** [LinkedIn](https://www.linkedin.com/in/danielthompson311/) / [Github](https://github.com/DanThomp507)

**Gresshaa Mehta, UI/UX Designer -** [LinkedIn](https://www.linkedin.com/in/gresshaa/) / [Twitter](https://twitter.com/gresshaa)

**Margaux Paradis, Product Manger -** [LinkedIn](https://www.linkedin.com/in/margaux-paradis/) / [Twitter](https://twitter.com/margaux_paradis)

### Why did you decide to build it

![DAO](https://user-images.githubusercontent.com/44700178/109560076-753e2200-7aa9-11eb-9230-5564f9c30b8a.png)

We set out to build Orca Protocol because we believe in the revolutionary power of the DAO. On chain software initiates an ecosystem that makes peer to peer governance a possibility, where organizations can function without the friction of traditional organizational models. 
However, the current systems are limited. Existing on-chain governance frameworks lack ways to meaningfully manage hierarchy and permissions. There is a usability problem with these setups which oftentimes result in voter apathy and misaligned voter incentives. A protocol which allows DAOs to easily create flexible rules and manage permissions is critical in order for on-chain governance to reach its full potential.

Our motivation in building Orca Protocol is to make the DAO vision a reality through allowing for DAOs to easily create customizable rules and manage permissions. We believe our adaptable protocol is a critical step toward on-chain governance reaching its full potential.

## Your Proposal

### Project description

![OrcaImg](https://user-images.githubusercontent.com/44700178/109560190-9272f080-7aa9-11eb-980a-b1a2effde117.png)

Orca Protocol is an efficient, Sybil-resistant DAO implementation using ERC1155 equipped with a simple UI dashboard to manage DAO proposals and allow on-chain voting for on-chain assets, all secured using Gnosis Safe.

We see Orca giving power to the original vision of the DAO where organizations pool their resources and collectively make decisions about how to allocate them in addition to providing the flexibility for new types of organizations to emerge and thrive. 

## Architecture

![image (3)](https://user-images.githubusercontent.com/44700178/110375560-21d75100-8020-11eb-80f5-46794fc7189e.png)


Orca is made up of pods: organizations that consist of a fixed number of member tokens each representing a single vote. A Pod can be small <10 or large >1000, and allows members to vote on membership requirements, fund allocations, and other on-chain activities. 

Pods are flexible and built modularly to accommodate infinite use cases including project governance, pooled investing, community management, and so much more. 

The Orca Protocol mints and distributes the pod's ERC 1155 member tokens. In order to claim a membership, one must meet the pod member requirements and rules. Each Pod is linked to a Gnosis Safe vault, that ensures it can securely hold and manage its collective on-chain assets.

![image (1)](https://user-images.githubusercontent.com/44700178/110375373-e177d300-801f-11eb-8328-03e5a95babfb.png)


Pod members can create proposals and vote on whether to execute. A proposal could be internal—defining requirements to hold membership—or external—performing on-chain actions such as deploying pod funds.

All proposals are executed on-chain by a network of third party users called shepherds. In exchange for Orca tokens, these shepherds ensure proposals are executed fairly and member requirements are being met.

### Tools

This project is built using Javascript and Solidity. To set up our dev environment we used Hardhat/Waffle, and main-net forking. We used ERC1155 to track our membership tokens, and rules are stored as Structs that get packed into transactions and executed at runtime. Each pod will be connected to a Gnosis Safe instance, and transactions are relayed through the safe. Additionally, we used Tenderly for some of the more complex debugging.

# Gnosis Safe Grant

![Frame_9](https://user-images.githubusercontent.com/44700178/110376379-1d5f6800-8021-11eb-994a-abad2bc4ac2f.jpg)

### **GECO Recommenders:** Graeme Barnes and Auryn Macmillan

## Timeline, Milestones and Deliverables

*Total* *Project Timeline: 4 months*

*Project Total: $100,000* 

![Untitled 6](https://user-images.githubusercontent.com/44700178/110376727-8941d080-8021-11eb-9270-2ef15bd8345c.png)
![Untitled 7](https://user-images.githubusercontent.com/44700178/110376732-8a72fd80-8021-11eb-912f-8b9f1ca62932.png)


**Phase I: MVP $52,000 [7 weeks]**

Deliverables:

- Front-End Design of V1: $16,000 [4 weeks]
- Front End Implementation of V1: $15,000 [5 weeks]
- Implement Gnosis Safe as multi-sig $6,000 [3 weeks]
- Pod hierarchies composability $9,000 [3 weeks]
- Clean up smart contracts $6,000 [2 weeks]

**Phase II: Network Development $33,500** 

Deliverables:

- Audit smart contracts: $12,000 [4 weeks]
- Bring to mainnet!: $1,500
- Add additional front-end features: $8,000 [2 weeks]
- $ORCA tokenomics: $6,000 [2 weeks]
- Shepherd incentives: $6,000 [2 weeks]

**Phase III: Optimize Usability $14,500**

Deliverables:

- Begin integration library: $10,000 [4 weeks]
- ZKP voting: $14,500 [4 weeks]

![Frame_5](https://user-images.githubusercontent.com/44700178/110376582-60214000-8021-11eb-977f-dbbd7f5d1440.jpg)


### Contact Us:

Twitter: [https://twitter.com/orcaprotocol](https://twitter.com/orcaprotocol)
Site: [https://www.orcaprotocol.org/](https://www.orcaprotocol.org/)
Github: [https://github.com/orcaprotocol](https://github.com/orcaprotocol)
Discord: [https://discord.gg/MRurnjD5](https://discord.gg/MRurnjD5)

