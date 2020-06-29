# Alfred Proposal

## Project Overview

### Project name
> Alfred

### Team members 
- Aaron Anderson
- Ken Hodler
- Morgan Sherwood
- Seth Goldfarb

### What project are you building 
Alfred is a cryptocurrency estate planner that allows people transfer their assets to a backup wallet or set of wallets after the system generates **proof-of-non-access** or **proof-of-death.** The dApp will help users set up their backup wallet or assign beneficiaries and access the funds once the system decides they're incapacitated or dead.

We offer two methods for determining whether or not someone can access their wallet:

1. Our decentralized inheritance solution generates **proof-of-non-access** when the user fails to check-in using our customizable **dead man’s switch**.

2. We will also offer an automated inheritance solution using a **live man's switch** that checks reliable sources of data to generate **proof-of-death**. Our first iteration uses data reported to the U.S. Social Security Administration and we plan to expand our geography according to demand.

Both methods incorporate flows for confirming and contesting the report of non-access or death.

Our goal is to develop tools that help prevent the loss of digital assets due to the loss of control over a particular set of keys. We will use this grant to fund development of our standalone dApp along with the Gnosis Safe app, have the software audited, and help cover the cost of subscription to the data service.

### Why did you decide to build it 
Helping people safely maintain custody of their digital assets remains one of the largest hurdles to the adoption of decentralized technologies. The value of lost cryptocurrency (sent to non-existent addresses or held in unreachable wallets) exceeds that of stolen cryptocurrency by a significant proportion (approximately 4x, according to our estimate).

Facilitating the inheritance of digital assets upon incapacitation or death represents a critical gap in decentralized key management.
Typically, there are two strategies for crypto inheritance:

1) Do nothing
2) Write down your keys with instructions on how to recover the assets

Unfortunately, "do nothing" is generally the default option. It is probably the one used by most people who own a moderate amount of digital assets and in these cases, the assets are lost when the holder passes away.

Writing down keys and instructions can work but introduces severe vulnerabilities with regard to OpSec. Wherever the keys are recorded, they are vulnerable to discovery and use by malicious third parties. Even when a trusted party is used, there are risks that the person or group will misbehave or handle the keys carelessly. Elaborate schemes can be used to overcome these vulnerabilities but the vulnerabilities are never completely mitigated and often these schemes introduce new vulnerabilities. 

Alfred introduces the concept of Perpetual Inheritance. This protocol increases the likelihood a digital wallet holder will be able to recover their assets in the event they lose access to their primary wallet by forcing them to prove their ability to access their primary wallet at regular intervals.

![](/Proposals/Alfred/PerpetualInheritance.png)
=======

### How long will it take 
We plan to launch our unaudited beta of Alfred August 1 with a full release and Gnosis Safe integration targeted for October 1.

### How much funding are you requesting  
$25,000

### How did you hear about the GECO
Twitter

## Your Proposal 
### Project description
We're applying for grants to support the ongoing development of Alfred and cover an audit of the smart contracts. The plan is to share an unaudited beta by the end of the summer and provide a full release the following quarter as both a standalone dApp and Gnosis Safe app. [Project Plan](Alfred/project-plan.md)

Our goals are to raise awareness of the issues around the self-custody of digital assets when using decentralized technologies and develop services that leverage Alfred to accommodate the needs of individuals and organizations maintaining custody of cryptocurrency and digital assets for various purposes. Some of these services may include:

- Helping individuals and organizations prevent the loss of digital wallets
- Helping individuals and organizations prepare for the death or incapacitation of loved ones or colleagues.
- Helping individuals and organizations share funds under various circumstances
- Helping fund managers design robust systems for maintaining custody of their own assets or advising clients on non-custodial management of their own assets.
- Helping businesses and non-profit organizations accept payments or donations of cryptocurrency.

### Features
- Digital Estate Inheritance

Estate owners designate how their assets will be divided among their chosen beneficiaries when the time comes.  An executor may be added to assist beneficiaries with the distribution process and to help in settling any outstanding loans.  The Alfred Estate dApp makes the process of inheritance distribution simple.

- Create or Sync Wallet

Create Wallet allows the user to make a Gnosis Safe that is automatically connected to and protected by their Alfred Estate. Sync Wallet allows users to connect an existing Gnosis Safe with their estate.  By connecting a Gnosis Safe Wallet to an Alfred Estate any assets stored in the wallet are protected.

- Wallet/Estate Recovery

The Alfred Estate smart contract is a Gnosis Safe Recovery Module. If access to a wallet is lost while the owner is alive, the Gnosis Safe can be recovered using the Alfred Estate. Recovery involves the assistance of beneficiaries and optionally the executor of the estate according to the owners prior specifications.

- Dashboard

  - Set/Edit Beneficiaries
  - Set Executor (if desired)
  - Distribute/Claim Funds

### Team description
- Aaron Anderson brings dApps to market as a dApp engineer and cofounder of Web3Devs and Ching!
- Ken Hodler is a senior engineer, formerly CEO and an early contributor at Keepkey (exited to ShapeShift).
- Morgan Sherwood is a dApp engineer with 25+ year career as a Python developer and algorithmic trader skilled in smart contract security analysis.
- Seth Goldfarb is a marketing professional who helps companies tell better stories about the development of blockchain and its applications.

The team began exploring this problem at ETHDenver 2020 and continued our work through the MetaCartel Dragon Quest, securing bounties from Kyber and Gnosis and winning 2nd Prize overall in the Dragon Quest along the way.

We are incorporated as a Wyoming-based LLC and operate using an Aragon DAO under a framework developed by Etherize.

### Timeline, Milestones and Deliverables

**Phase I**

**Deliverables**
- Complete smart contracts and front-end
- Launch (unaudited) beta version for testing

**1 Month - $6250**	

**Phase II**

**Deliverables**
- Audit smart contract
- Consult legal counsel
- Interview users

**1 Month - $12500**

**Phase III**

**Deliverables**
- Iterate on UI
- Address concerns revealed in audit
- Launch full release and Gnosis Safe app

**1 Month - $6250**
