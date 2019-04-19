# Alice Dapps | Gnosis Ecosystem Fund
Crypto Superapp as a path to reduce friction, increase usability and accelerate mass consumer adoption

## Project Overview

### Project name
> Alice

### Team members 

Alice team members can be found here: https://www.alicedapp.com/team

Mark Pereira - Fullstack developer and Product Design

Daniel Bar - Web3 UX Research and Project Manager

### What project are you building 

We are building a crypto super app. It's a mobile app that allows other crypto applications to build mobile applications in React Native into our application. We are heavily focused on User Experience and bringing more utility to the space that needs it the most, which is the Blockchain mobile space. 

### Why did you decide to build it 
We decided to build it because we were unhappy with the current solutions out there and were yearning for mobile native apps that had the utilities available on web. This is after extensive research in the space around user's experiences and developer's problems.

### How long will it take 

6 Months

### How much funding are you requesting  

$100,000

### How did you hear about the GEF

We met Stefan in the MetaCartel dinner at DEVCON and he informed us on the GECO program.

## Your Proposal 

### Project description
Our proposal is 1. to use the Gnosis Personal Mulitisig as the de facto smart contract account for the Alice Wallet to be able to utilise Layer 2 UX and scaling solutions that bring better experiences to users 2. To build a mobile native interface for the DutchX exchange so that Gnosis can access users who are spending most of their time on mobile. 


#### Abstract


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

**Mark Pereira**: Cofounder, Fullstack developer with experience building and architecting web and mobile dapps. Before the web3 space, he was a web developer at a variety of dev agencies.

Linkedin: https://www.linkedin.com/in/markspereira/

**Daniel Bar**: Cofounder, Project Manager. Daniel has experience working as an R&D Engineer in the semiconductor industry and nanoelectronics. Deeply rooted in the Chinese cryptocommunity and leading the bitfwd community in APAC region. 

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
