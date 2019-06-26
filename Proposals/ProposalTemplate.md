# Proposal Guideline 
_This is a guideline on how to best structure your proposal._

## Project Overview

### Project name
> Identity
### Team members 
> Dennison Bertram
> Seth Fork
### What project are you building 
> An Identity contract on Ethereum that can represent users as a first-class citizen in Ethereum. 
ERC725 complient, MetaTransaction enabled, and Gnosis Multi-Sig for Social Recovery, 2FA, transferable accounts, and fine grain permission controls. 
Identity can execute aritrary function calls, and both create and create2 contracts. An Identity also stores metadata allowing the user- be it organizations,
individuals, daos or otherwise, to keep a public (or encrypted) record of documentation related to the identity. 
### Why did you decide to build it 
> I have been working on two projects: A Doctor Dao where patients can request Vaccination records from DAO doctors, and a Digital art Archival tool for artists. 
In the process of building these two projects I realized that there was an overlapping base compoment that was missing: Identity. Both the Doctor Dao and the
artist project needed a way to represent an Identity on the blockchain with associated MetaData. In the case of the Doctor Dao- doctors need to supply their 
public credentials stored in metadata, where as the patients can link themselves through familly in encrypted metadata and medical notes for vaccinations. 
In the case of Artists, a singular contract that could act as the authoritative source of an artists archive needed the ability to create new token lineages that 
represent their art, along with Metadata to describe themselves and create a catalogue. 
For both these projects, I need an Identity. Something easy to use (MetaTxns for onboarding issues), but also something forgiving- Gnosis multisig for Social Recovery
and flexible but secure permission model. 
### How long will it take 
> The project I have broken down into phases. Each phase will incrementally improve the usability and developer experience of the Identity platform. 
I estimate 1 quarter for each phase, with a total of 4 quarters to deliver a polished, production level product accesible to the average front-end *developer*. 
Note that my target is not limited to *web3* developers. My goal is to create something simple and open for developers.   
### How much funding are you requesting  
> Each phase has a different estimated requirement for funding. I have already finished a working proof-of-concept so the first phase the funding I am requesting is lower
than the others which have yet to be started. 
Phase 1: Completion of the base Solidity Code + testing: $2,500
Phase 2: Creation of a Javascript library part 1: A javascript API for interacting with the Identity smart contract code. $6,000
Phase 3: Creation of a Javascript library part 2: Gasless, keypair-less usage for web2 style onboarding: $3,000
Phase 4: Documentation and Tutorials: $1,500
Phase 5: Auditing: Unsure, the goal is a community project. So a community audit should be requested. 
### How did you hear about the GECO
> From the Twitter.

## Your Proposal 
### Project description
_Outline a detailed description of your project, why you chose to build this project, the overall goal and future outlook of your project and why we should fund you._
Identity is a first-class citizen as a smart contract. It builds upon the draft ERC725 standard and expands it to create an Idnetity that can practically represent a user or
organization on the blockchain- without needing them to hold Eth or use metamask. 
Onboarding regular users to Ethereum requires giving users an experience that does not require eth or metmask to securely interact with. There are many use
cases for ethereum that largely do not revolve around finance, but are underserved by the current community tools. Identity is to be an open source tool that is
platform agnostic, any developer can build upon it free of charge. Identity is a *building* block for more inclusive, low-friction blockchain backed applications. 
Identity seeks to build a free, open source building block for developers. Identity is not the business model in and of itself. It is community software so everyone
can build more powerful, more inclusive, applications. 
### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._
Identity is built using ZeppelinOS. This allows for itterative development, modularity via EVM packages of on-chain code libraries, and optional upgradability of contracts. 

The smart contracts are written using solidity. The Javascript library is written using Nodejs.

Identity is compatible with the ERC725 proposal for Identity contracts. 

MetaTransactions are powered by the Gas Stations Network which will be released soon by Zeppelin, TabooKey and the Gas Stations Network Alliance

Social Recovery, ownership portability, and personal account recovery are provided by Gnosis multisig. The javascript library will give an easy way to use these functions. 

OpenZeppelin Roles are used to guard permssions. 

MetaData is stored in contract with a caching feature to minimize API calls. 

Javascript library will utilize IPFS/Swarm for storage of metadata and ecnryption. 

### Team description
_Who are your team members, what is your background and what you built before._
Dennison Bertram - 'founder' - I am developer Advocate at OpenZeppelin. I build numerous tutorials for our products, and have a number of soon-to-be released demo applications
for MetaTransactions and the Gas Stations Network. I originally got into crypto in 2011 and I created the first Bitcoin exchange in the czech republic called BuyBTC.cz in 2012.
I have spoken at a number of conferences as developer advocate and run programming workshops for solidity. I was MC of ETH New York and was a prize winner at the ETH Buenos Aires hackathon, MakeDao prize winner at Status IM Hackathon durring Devcon 4, and WindingTree durring Devcon 4 hackathon among others. I am a member of CryptoNYC.

Seth Fork - Member CryptoNYC. State Sauce: https://github.com/sethfork
https://github.com/statesauce/redux-saga-web3

### Timeline, Milestones and Deliverables
_Detailed description of your timeline milestones and the corresponding payouts_
Note: This is budgeted like a renumerated community project. 
It is budgeted as a part-time project with concrete goals and milestones.

**Phase I**  			_Outline the different phases_
Phase 1: Completion of the base Solidity Code + testing: $1,500

In this phase the working code of the first version is completed. Currently the code is at Alpha status and is functional with a limited set of passing tests for some of the more 
challanging features (Create2 contract creation, arbitraty code execution)
**Deliverables** 			_What features will be implemented_

A working v1 beta-version of the code. All base functionality completed:

Modularity: Functionality is implemented via ZeppelinOS EVM packages. Each group of functionality is isolated in an individual EVM package to create a composable application. 

Draft ERC725 functionality: (following: https://github.com/ethereum/EIPs/issues/725)

MetaTransaction support: Incorporation of Gas Stations Network 

Gnosis MultiSig integration: Support for Social Recovery and various recovery mechanisms. 


**Time and Price Estimate**	
$2500

I expect this to take 3 weeks. Most of the Alpha code is completed and working. There is substantial refacotoring to do, but much of the code builds upon code already
developed by the community and composes it. The majority of the work here is designing a more complete set of tests. 

**Phase II**  			_Outline the different phases_
Creation of a Javascript library part 1: A javascript API for interacting with the Identity smart contract code. 

In this phase a nodejs library is built to simplify the process of interacting with Identity. Currently things like executing arbitrary code via smart contract are cumbersome
for most developers to implement. Creating and managing `create2/create` contract creation requires a number of utility functions and various steps to do, which make it
harder to work with. 

**Deliverables** 			_What features will be implemented_
Javascript library for creating and interacting with Identities. 

1. Creation of Identities
2. Creation/Execution of arbitrary code via Identities
3. Creation, updating metadata for Idnetities. 
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

**Time and Price Estimate**	_How long will it take and what is the estimated price_
$6,000
6-8 weeks

**Phase III**  			
Phase 3: Creation of a Javascript library part 2: Gasless, keypair-less usage for web2 style onboarding:

IPFS/SWARM integration for storage and retreival of Metadata. 

Metadata Caching for reducing API usage. 

The effectivness and usability of MetaTransactions depends on developers being able to effectively keep track of Ephemeral use keypairs. This phase will 
create tools to help developers do this in a simple, web2 style manner using technologies web2 developers are already familiar with. This should not be the
core of any effective decentralized system, but is nessesary for the onboarding process. 

I understand this does not feel "totally crypto" but it's very nessesary for practical onboarding of developers and users. Any DApp can require that a user, 
after 5 trasnactions (for exapmle) must setup a new Metamask and transfer full control to the users responsiblity. However we loose users by requiring 
Metamask, 12 words, KYC for ETH, etc... at the very start. 

***Delibverables**

Javascrip front end Library for generating and managing Ephermeral Keypairs
Metadata Caching with IPFS
Demo express server for encrypting recovery keypairs
Demo OATH integration for recovery keypairs. 


**Time and Price Estimate**
$3000
4 weeks. 

### Others	 
Anything else you want to share with us
