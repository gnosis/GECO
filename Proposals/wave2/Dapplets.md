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
*Dapplets* is a research- and infrastructural project enabling new business models and mass adoption for Dapps. It allows embedding ethereum based actions into existing web2 legacy websites and communities like Twitter. Moreover, the project fixes current flaws in the web3 architecture, repairing [WYSiWYS](https://en.wikipedia.org/wiki/WYSIWYS) property of secure signing process and make it more secure and seamless.

### Why did you decide to build it
I (Ethernian) was looking for ways to implement ethereum based workflows on the top existing communities. It is essential for Ethereum Governance (Signaling) and for [routing EIPs](https://ethereum-magicians.org/t/decentralizing-eip-workflow/1525)  between specialized communities. It turned out, that the current secure signing infrastructure based in current web3 architecture doesn't support existing legacy sites.
The broken [WYSiWYS](https://en.wikipedia.org/wiki/WYSIWYS) was the second driver to start the project.
  

### How long will it take

1. Phase 1: a Gnosis MVP - 2 months
1. Phase 2: public beta - 3 months
1. Phase 3: public release - 3 months

  

### How much funding are you requesting
1. Phase 1: 12000 euro
1. Phase 2: 18000 euro
1. Phase 3: 18000 euro

Total: 48000 euro


### How did you hear about the GECO

personal conversation in FullNode with Dmitry Bespalov and then with Mareen Gläske and Tobias Schubotz.

## Your Proposal

### Project description

The Dapplets proposal improves the current web3 architecture by splitting web3 workflows into two groups: the “UX-focused” and the “Security-focused” and executes the latter workflows in the Signer’s secure environment. For usual Dapps the architecture solves "UX vs. Security" trade-off and achieves both: UX and security. For an existing legacy website it allows defining ethereum actions running in Signer even if the site has no web3 support at all. It means, now we can reach millions of users on sites like Twitter. 

More generally speaking, the Dapplets proposal allows setting up an ethereum based incentivization layer on the top of existing web2 communities.

Legacy site support makes the _Dapplets_ to the vehicle for mass adoption and creates this way an incentive for wallet devs to implement the standard.

In particular, a dapplet integration with Gnosis-Safe will allow users to create Prediction Markets seamless in the context of the website where the User is currently on. For example, the User can join a Prediction Market about US election results or create a bet against some fake news _directly from the news site he or she is reading_ even if the news site has no web3 support at all. I have already discussed the implementation details with Dmitry Bespalov: it looks positive.

### Features

As for now, we are planning to create a browser plugin for injecting dapplet controls. We use WalletConnect to pair the wallet and the browser. A dapplet description language (a Dapplet DSL) is to be defined but will be a subset of HTML or Markdown or similar.
Dapplet Auditor Community planned to be a DAO or TCR.

### Team description

*Dmitry Palchun (Ethernian)* - former java developer with more than 25 years of experience. Since 2015 - an ethereum developer and architect. Implemented ethereum based PoC projects and researched blockchain business cases at Lufthansa. In 2017 created independently all contracts around Santiment ICO, token and subscriptions. [Active in Ethereum Magicians](https://ethereum-magicians.org/u/ethernian) forum. An author of Dapplets proposal.
Based in Hamburg.


*Ralf Sturm (meekmocha)* - an experienced UI/UX designer. 20+ years of experience.
UX tests and guidance for Olympus audio recorder, UX/UI for interactive GPS driven outdoor games, UI/UX for Jabber-based messenger, various network game designs since 1999, UX/UI for Cycosmos (pre-Facebook).
DJ and musician. 
Based in Hamburg.

*Alexander Sakhaev* - fullstack developer at SkillUnion. Implemented a Dapplets PoC at ETHParis hackathon in Paris, as well as various pre-Dapplets experimentations like Metamask forking & hacking. 3+ years of experience.
Based in St.Petersburg.

*Andrey Chukhonin* - fullstack developer at SkillUnion. A lot of industrial ERP integrations with 10+ years of experience.
Based in St.Petersburg.


SkillUnion is a traditional IT company in St.Petersburg, founded by Sergey Palchun. It implements ERP systems for industrial customers.

### Timeline, Milestones and Deliverables

The project is divided into several modules:

* *Injector:* a browser plugin loading and injecting controls into the website depending on context.
* *Protocol:* a DSL for dapplets and controls definition.
* *Infrastructure:* to maintain the dapplet's security status and for serving the data.
* *Wallet support:* implement the Dapplets support in Wallets/Signers.
* *TestCases:* real live dapplets and business cases, creating incentives for Wallet Devs to adopt the Dapplets protocol.
  

**Phase 0** 
Weeks of hacking around Metamask and TCR.
A quick and dirty [implementation was made at ETHParis hackathon](https://twitter.com/Ethernian/status/1104596777519452160) based on WalletConnect. 

*<==== YOU ARE HERE =====>*

**Phase I** 
Gnosis MVP: a supporting one gnosis use case as a test.
**Deliverables**
* Injector: a browser plugin loading and injecting context dependent controls.
* Protocol: threats and security model research for secure signing; create a simple DSL to define controls and dapplets.
* Infrastructure: simplified and mostly centralized audit infrastructure and data delivery.
* Wallet support: one wallet PoC integration (Gnosis-Safe would be great).
* TestCases: one TestCase to be defined together with Gnosis Team 
(like Twitter or news feeds integrations).  

**Time and Price Estimate** 
2 months, 12000 Euro

  

**Phase II** 
First public beta: support for many independent dapplets and authors. 
**Deliverables**
* Injector: security levels, checks and events; user-based favorites and ignores
* Protocol: implementing the security model and DSL.
* Infrastructure: simple decentralized audit and security management. Simple project web site, dapplet documentation and developer community.
* Wallet support: dapplet container implemented in Gnosis-Safe.
* TestCase: Gnosis test case: rolling out and collecting feedback.

**Time and Price Estimate** 
3 months, 18000 Euro
  

**Phase III** 
First public release.
**Deliverables**
* Injector: implement fixes and changes from Phase II.
* Protocol: implement fixes and changes from Phase II.
* Infrastructure: decentralized audit and security management with economic incentives.
* Wallet support: second wallet integration. Documentation.
* TestCases: one more UseCase (to be defined).

**Time and Price Estimate** 
3 months, 18000 Euro
  

### Others

Technical and business details of the Gnosis-Safe integration were already discussed with Dmitry and Tobias. 
It would be great to become a chance to bring ideas to reality. 

Technical Whitepaper: http://bitly.com/dapplets-part1

PoC video: http://bitly.com/dapplets-poc-video

Forum discussion: http://bitly.com/dapplets-forum


PoC github (created at ETHParis Hackathon):

https://github.com/skillunion/dapplet-extension

https://github.com/skillunion/walletconnect-mock-wallet

https://github.com/skillunion/dapplet-static
