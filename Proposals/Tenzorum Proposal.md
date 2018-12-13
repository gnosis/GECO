# Tenzorum Project | Gnosis Ecosystem Fund
_A gasless onboarding experience to support seamless UX ._

## Project Overview

### Project name
> Tenzorum Project

### Team members 

All Tenzorum team members can be found here: https://tenzorum.org/team/

Moritz Neto - General Manager and UX Lead

Radek Ostrowski - CTO and Tech lead 

Mark Pereira - Fullstack developer and Product Design

Daniel Bar - CEO and Project Manager

### What project are you building 

Tenzorum is focused in building a complete end-to-end onboarding kit for the decentralized web, to empower the developer community to build friendly and familiar applications using Blockchain Technology and give users a secure portal to the web 3.0.

### Why did you decide to build it 

Our decision comes from the fact that the onboarding experience for applications using Blockchain is completely broken. If we are talking about mass consumer adoption and hitting the mainstream with decentralized technology, it is naive to assume that people will interface with the complexity of our current systems to simply start using an application.

If our main priority as a community isn’t to build friendly technology that empowers people, we are going in the wrong direction.

We believe that creating this system where new users don’t have to go after ETH and the insane KYC process to execute simple on-chain functions or send randomly acquired ERC20s, can liberate the growth and potential of the Ethereum community and all applications.


### How long will it take 

6 Months

### How much funding are you requesting  

$120,000

### How did you hear about the GEF

Met Stefan, Gnosis CTO at DEVCON and found a lot of synergies in our vision. 🏄

## Your Proposal 
### Project description
#### Abstract
We will be building a secure, easy-to-use user account for the Ethereum blockchain. A user's "blockchain account" will be a Gnosis Safe Multisig wallet located via a human readable ENS name much like a username. A user will deploy this account through a seamless onboarding solution powered by MetaConnect and our onboarding kit [tenzorum SDK](https://github.com/Tenzorum/tenzorum). 

A user will then be able to interact with his "account" immediately without having required ETH because of the use of meta-transactions and our service node network in this architecture. This avoids the pain and complexity of a user having to acquire ETH to start using applications.

#### Project elements:
1. A connection application called MetaConnect that leverages and displays all the elements being built to showcase the potential of meta transactions (Relayed tx) being built as a progressive web-app, where users are interactively onboarded and deploy a Gnosis SAFE multisig wallet as part of the process. We see the integration of Gnosis SAFE as an integral piece of web3 security, particularly with recovery configuration and the ability to remove trusted party recovery methods. 

2. An open SDK to allow developers to seamlessly deploy and use:
  
      a. Ephemeral Keys - Key that are used and get discarded or replaced with a stable key in the process of application onboarding.
  
      b. A personal multi-sig (GNOSIS SAFE) - A wallet contract that connects between the various devices users interact with and serves as the stable keychain for users' relevant longer term assets holding as well as access recovery.
  
      c. Personal ENS Domains (TENZ-ID) - a 1 click ENS subdomain factory that allows users, programs and developers to interact with human readable Ethereum addresses. The initial mainnet implementation can be found on [tenzorum.org/tenz_id](https://www.tenzorum.org/tenz_id).
  
      d. Meta-Transactions (Relayers) - Transaction that are signed off-chain and are relayed to the network via a proxy node that pays the gas fees.    
  
3. Tenzorum Service Node Network - A decentralized relayer network to support meta-transactions with token rewards connected to DutchX as a liquidity provider. An initial test implementation currently runs in single node mode. Research of the cryptoeconomic models to expand and build a relayer node network in order to create a market for a permissionless layer 2 economies.


#### Further Research and Collaboration
1. Social Recovery to complement the personal Gnosis SAFE, user friendliness and safety of user funds.


### Features

- EIP 1077 implementation - Universal Logins + Relayer Network

- Gnosis SAFE integration into Tenzorum SDK/Universal Logins SDK

- User will be able to deploy a Gnosis SAFE from MetaConnect app.

- Developers will be able to integrate Gnosis SAFE into their applications easily.

- Relayers will be able to convert the rewarded tokens using DutchX.

- All the work and achievements will be broadcasted as tutorials and development guides.

### Associated Team Members Description

**Moritz Neto**: Cofounder of Tenzorum Project, Product designer and Growth Manager. Have directly educated more than 300k people about smart contracts and Blockchain Technology with his content.

Linkedin: https://www.linkedin.com/in/moritzneto/


**Radek Ostrowski**: Blockchain Engineer particularly interested in Ethereum and Smart Contracts. In the fiat world, experienced in Big Data and Machine Learning projects. Triple winner in two different international IBM Apache Spark competitions and awarded a prize in ConsenSys hackathon. Co-creator of PlayStation 4 backend.

Linkedin: https://www.linkedin.com/in/radekostrowski/

**Mark Pereira**: Fullstack developer with experience building and architecting web and mobile dapps. Before the web3 space, he was a web developer at a variety of dev agencies.

Linkedin: https://www.linkedin.com/in/markspereira/

**Daniel Bar**: CEO and Project Manager. Daniel has experience working as an R&D Engineer in the semiconductor industry and nanoelectronics. Deeply rooted in the Chinese cryptocommunity and leading the bitfwd community in APAC region. 

Linkedin: https://www.linkedin.com/in/dtbar/

## Timeline, Milestones and Deliverables

Encourage Gnosis SAFE and DutchX Adoption. 

Note, the below milestones can be achieved in parallel.

### Integration of Gnosis SAFE functionality into the SDK component ($25k - 2 months)
Incorporate SAFE into the SDK (leveraging Universal Logins), thus providing anyone the possibility of integrating SAFE into their applications. This will include all the wallet operations - checking balances, sending ETH, sending tokens, etc. Existing SAFE functionality will be replicated and adapted and a developer friendly SDK interface to SAFE will be created. The ease of use of the SDK will be enforced by the work in sections below. The result of this will be an open sourced SDK including Tenzorum, Universal Logins and Gnosis SAFE functionality.

### User and developer experience work ($10k - 1 month)
Prepare documentation and interfacing guidlines for users to be able to seamlessly use and understand Gnosis SAFE.
Prepare documentation for developers explaining all the functionalities of the Gnosis SAFE through the SDK including
code snippets and example implementations. The work of demonstrating the use of the SDK is described in the following section. 
The result of this work will be several blog posts and developer documentation on SAFE and it's usage via the the SDK.

### Integration of Gnosis SAFE into [MetaConnect](https://www.metaconnect.org) ($20k - 1.5 months)
MetaConnect allows even non-blockchain aware users to be seamlessly onboarded to Ethereum. 
Demonstrate the use of the SDK by integrating it into MetaConnect app. This will include an option to have SAFE created via sponsored meta transaction and the use of TENZ-ID to be associated with the SAFE instance. Additionally, all usual SAFE operation will be available as per SDK. We consider MetaConnect as a vehicle for constantly aquiring more users keeping them engaged. This will offer continuous exposure of Gnosis products to Tenzorum current and future audience. 
The result of this work will be MetaConnect app offering the creation of Gnosis SAFE with an associated TENZ-ID and all SDK SAFE features.

### Leverage MetaConnect to feed Social Recovery module of Gnosis SAFE ($10k - 1 month)
Currently, SAFE owner has to know the exact wallet address of their friends. This could be simplified by using TENZ-ID 
of any of the existing connections and build out into the app. As a result, users of MetaConnect will be able to choose which of their connections could become their SAFE social recovery friends.

### Relay Service Network deployment ($40k - 3 months)
Build a relayer nework capable of executing meta transaction which are either sponsored or paid for in ETH or ERC20 tokens. Relayers are coded in Node.js and can be easily run and deployed by anyone using ElectronJs App (currently it's available via Docker or NPM).
As a result, users not holding any `ETH` will be able to use their SAFE and pay for any operations in ERC20 tokens. Anyone can participate in the network as a relayer and earn meta transaction fees.

### Liquidity reserves integrations with DutchX ($15k - 1 month)
The relayers which are accepting ERC20 tokens as fee for their services and gas cost will be interested in converting them back to `ETH`.
Develop backend integration with DutchX to allow relayers to convert their fee tokens. This will result in extension of relayer code enabling the owners to convert their tokens into `ETH` using fair price as provided by DutchX.
