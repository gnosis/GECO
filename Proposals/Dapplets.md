# Dapplets: improved secure signing protocol

## Project Overview

### Project name

[Dapplets](https://medium.com/@Ethernian/dapplets-part-1-introduce-new-dapp-architecture-for-better-ux-and-security-75a4881b4765)

### Team members

Dmitry Palchun (AKA [@Ethernian](https://ethereum-magicians.org/u/ethernian)) - ethereum developer, founder
Ralf Sturm - UI/UX designer, frontend developer
Alexander Sakhaev (from SkillUnion) - fullstack developer
Andrey Chukhonin (from SkillUnion) - fullstack developer

staffing from SkillUnion may vary.

### What project are you building
*Dapplets* is a research- and infrastructural project enabling new business models and mass adoption for Dapps. It allows to embed ethereum based actions into existing web2 legacy websites and communities like Twitter. Moreover, the project fixes current flaws in the web3 architechture, repairing [WYSiWYS](https://en.wikipedia.org/wiki/WYSIWYS) property of secure signing process and make it more secure and seamless.

### Why did you decide to build it

  

### How long will it take

1. Phase 1: a Gnosis MVP - 2 monthes
1. Phase 2: public beta - 3 monthes
1. Phase 3: public release - 2 monthes

  

### How much funding are you requesting
1. Phase 1: 12000 euro
1. Phase 2: 18000 euro
1. Phase 3: 12000 euro


### How did you hear about the GECO

personal conversation in FullNode

## Your Proposal

### Project description

Dapplets proposal improves the current web3 architecture by splitting web3 workflows into two groups: the “UX-focused” and the “Security-focused” and executes the latter workflows in the Signer’s secure environment. For usual Dapps the architecture solves "UX vs. Security" trade-off and achieves both: UX and security. For existing legacy website it allows to define ethereum actions running in Signer even if the site has no web3 support at all. It means, now we can reach millions of users on sites like Twitter. 

More generally speaking, Dapplets proposal allows to set up an ethereum based incentivization layer on the top of existing web2 communities.

Legacy site support makes the _Dapplets_ to the vehicle for mass adoption and creates this way an incentive for wallet devs to implement the standard.

In particular, dapplet integration with Gnosis-Safe will allow users to create Prediction Markets seamless in context of the website where the User is currently on. For example, the User can join a Prediction Market about US election results or create a bet against some fake news _directly from the news site he or she is reading_ even if the news site has no web3 support at all. 

### Features

_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._

### Team description

*Dmitry Palchun (Ethernian)* - former java developer with more than 25 years experience. Since 2015 - an ethereum developer and architect. Implemented ethereum based PoC projects and researched blockchain business cases at Lufthansa. In 2017 created independently all contracts around Santiment ICO, token and subscriptions. [Active in Ethereum Magicians](https://ethereum-magicians.org/u/ethernian) forum. An author of Dappets proposal.
Based in Hamburg.


*Ralf Sturm (meekmocha)* - an experienced UI/UX designer and frontend developer with more than 20 years experience. DJ and musician. 
Based in Hamburg.

*Alexander Sakhaev* - fullstack developer at SkillUnion. Implemented a Dapplets PoC at ETHParis hackaton in Paris, as well as various pre-Dapplets experimentations like Metamask forking & hacking. 
Based in St.Petersburg.

*Alexander Sakhaev* - fullstack developer at SkillUnion. Implemented a Dapplets PoC at ETHParis hackaton in Paris, as well as various pre-Dapplets experimentations like Metamask forking & hacking. 
Based in St.Petersburg.

*Andrey Chukhonin* - fullstack developer at SkillUnion.
Based in St.Petersburg.


SkillUnion is a traditional IT company in St.Petersburg, founded by Sergey Palchun. It implements ERP systems for industrial customers.

### Timeline, Milestones and Deliverables

The project is splitted several modules:

* *Injector:* a browser plugin loading and injecting controls into the website depending on context.
* *Protocol:* a DSL for dapplets and controls definition.
* *Infrastructure:* to maintain the dapplet's security status and for serving the data.
* *Wallet support:* implement Dapplets support in Wallets/Signers.
* *TestCases:* real live dapplets and business cases, creating incentives for Wallet Devs to adopt the Dapplets protocol.
  

**Phase 0** 
Weeks of hacking around Metamask and TCR.
A quick and dirty [implementation was made at ETHParis hackathon](https://twitter.com/Ethernian/status/1104596777519452160) based on WalletConnect. 

*<==== YOU ARE HERE =====>*

**Phase I** 
Gnosis MVP
**Deliverables**
* Injector: a browser plugin loading and injecting context dependend controls.
* Protocol: threats and security model research for secure signing; create a simple DSL to define controls and dapplets.
* Infrastructure: simplified and mostly centralized audit infrastructure and data delivery.
* Wallet support: one wallet (Gnosis-Safe would be great).
* TestCases: one TestCase to be defined with Gnosis.  

**Time and Price Estimate** 
2 Monthes, 12000 Euro

  

**Phase II** 
First public beta.
**Deliverables**

* Protocol: implementing security model and DSL.
* Infrastructure: simple decentralized audit and security management. Project WebSite and simple developer community.
* Wallet support: one wallet (Gnosis-Safe would be great).
* TestCase: one UseCase (to be defined with Gnosis).

**Time and Price Estimate** 
3 Monthes, 18000 Euro

  

**Phase III** 
First public release.
**Deliverables**
* Injector: implement public feedback.
* Protocol: implementing security model and DSL.
* Infrastructure: simple decentralized audit and security management.
* Wallet support: one wallet (Gnosis-Safe would be great).
* TestCases: one more UseCase (to be defined with Gnosis).

**Time and Price Estimate** 
2 Monthes, 12000 Euro

  
  

### Others

Anything else you want to share with us