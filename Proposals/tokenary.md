# Proposal Guideline

## Project Overview

### Project name
Tokenary

### Team members
* Vadim Zakharenko  — vadim.zakhar42@gmail.com — https://github.com/vadimantiy
* Igor Shmakov — shmakoff.work@gmail.com — https://github.com/shmakovigor
* Ivan Grachyov — mail@grachyov.com — https://github.com/grachyov
* Ilya Lozhkin — mini223@yandex.ru —  https://github.com/lonesta
* Olga Kolekonova —  anoniav@gmail.com — https://github.com/duprass
* Vadim Koleoshkin — vadim@zerion.io — https://github.com/rockfridrich  

### What project are you building
We are building Tokenary, a simple and seamless cross-device ethereum wallet for crypto newcomers. Our main priorities are security and usability. We want to help users interact with the Ethereum network and DApps in a simple, straightforward way while preserving their favorite features like cross-device sync, push notifications, and extra layers of security (Face ID, Touch ID, KeyChain, etc.). Our initial target market is the crypto-enthusiast Apple user that desires Apple’s simple UX in all of their interactions with the crypto world, which is currently impossible to find—especially for decentralized finance applications. Eventually, we plan on building complementary Android and web-client interfaces to reach additional market segments.
In Summer 2017, our core team won second place at the Qtum hackathon in Moscow and have been working full-time on Tokenary ever since. In Summer 2018, we published a macOS app in the Mac App Store to complement our existing iOS application. After some additional research and user-testing, we identified a need for Safari-based solution for interacting with Dapps from our wallet. This Safari extension injects a Web3 provider into the Tokenary interface to transmit signing requests.
We are always on the lookout for the latest UX protocols like WalletConnect and implement them to make the cross-device wallet experience even better.

### Why did you decide to build it
When we first started using the Ethereum network in 2016, we faced many usability problems common to new technologies. In an attempt to address them, during the Qtum hackathon in Moscow in the summer of 2017, our team developed a prototype of a simple wallet application.

We want to make interaction with Ethereum smart contracts, tokens and DApps as familiar as possible with all the features we love from the Apple Ecosystem — cross-device sync, push notification and extra layers of security (Face ID, Touch ID, KeyChain, etc.). Current UX solutions do not offer these features or were implemented on a single platform without the crucial cross-device experience.

### How long will it take
We are continuously working on our clients for mobile, desktop and web. Here is our roadmap for 2019:

**Q1-2019**
* Safari extension to enable DApp interaction
* In-app and web explorer to make transactions more understandable for the new crypto user
* In-app token exchange with the best rates across different DEXs
* ENS support

**Q2-2019**
* Meta Transactions for alternative gas payments
* Universal Login or another simple key-recovery system
* Cross-device transaction memo synchronization with IPFS
* Address book and user profile support
* Asset information discovery and in-app educational content

**Q3-2019**
* Android client parity with iOS
* Major hardware wallet support for macOS
* P2P exchange for NFTs and other assets
* Transaction signing from keyless devices.

**Q4-2019**
* Apple Pay purchase of Ether and various stable coins (DAI)
* In-app crypto purchasing with credit cards/apple pay  
* Adding Bitcoin and WBTC bridge support
* Sending crypto via messages and other channels to onboard new users
* Light client implementation

### How much funding are you requesting  
$60 000

### How did you hear about the GECO
We met Stefan George at a DeFi meetup in Berlin and saw mentions of the program on Twitter

## Your Proposal

### Project description
We want to give users the ability to use shared accounts to manage their crypto assets. Setting up a shared account to hold Ethereum assets is a tricky process now. Besides additional security that a shared account gives, it allows users to manage their funds together which is hard to do within the existent financial infrastructure (i.e. bank accounts). Using our existing software, iOS, macOS and web wallet interfaces, we want to provide our users with the best user experience. We want to make the process of submitting and confirming transactions as fast and convenient as possible.

### Features
* Shared account creation (deployment of a contract with required parameters)
* Invitations to a shared account (notifications and email requests)
* Sync of shared accounts addresses (sync via iCloud, local storage, etc.)
* Wallet configuration (setting owners, limits, number of approvals)
* Notifications (on payment requests and approvals)
* Shared memos about transactions (with IPFS and shared key cryptography)
* Transaction creation and execution (ETH, ERC-20, ERC-721)
* List of transactions

### Team description
The 6-person Tokenary team is purely technical and includes developers with experiences in various industries. Most of the team members have a CS or Mathematical degree from the top Russian universities.

**Ivan Grachyov** (Product manager & iOS developer)
* Apple WWDC scholarship winner
* Bachelor in Computer Science from Lomonosov Moscow State University
* Founded and developed [Emoji Cosmos](https://www.producthunt.com/posts/emoji-cosmos)

**Vadim Zakharenko** (iOS developer)
* Google intern
* Apple WWDC scholarship winner
* Bachelor of Computer Science at Lomonosov Moscow State University
* Competitive programming olympiads winner

**Igor Shmakov** (macOS & iOS developer)
* Founded and developed [Arseny](https://itunes.apple.com/ru/app/id1340250301), [Spont](https://itunes.apple.com/us/app/spont-make-events-meet-new-people/id1125189088?mt=8)
* Bachelor of Computer Science and Engineering at National Research Nuclear University MEPhI
* Co-author of [Classifiers based on Bayesian neural networks](https://ieeexplore.ieee.org/document/7910653)

**Ilya Lozhkin** (Fronted & Backend developer)
* [WalletConnect PHP bridge open source](https://github.com/Tokenary/laravel-walletconnect-bridge)

**Olga Kolekonova** (Android developer)
* Software Engineering Degree from Higher School of Economics

**Vadim Koleoshkin** (Product manager & Backend developer)
* Founder at [Zerion](https://zerion.io) (Trustless banking) & Jufy (100+ corporate development projects)
* Business informatics Master’s degree from Higher School Of Economics
* Contributor to Web3Swift (https://web3swift.io/)

### Timeline, Milestones and Deliverables

**Phase 1** — Alpha\
**Deliverables** — Creating accounts, Adding owners, Transacting\
We plan to release the basic flow of a multisig creation with predefined owners, signing and sending ETH and ERC-20 transactions (iOS and macOS)\
**Time and Price Estimate** — 2 months (20 000$)

**Phase 2** — Beta\
**Deliverables** — Invitations, Synchronization, Settings
The next step will be to enable inviting of other owners usign signed messages delivered via email or messengers. We will also implement synchronization of the multisigs list via iCloud to prevent users from losing their addresses. Additional settings will be available in the settings tab to make limits and a number of confirmations configurable.\
**Time and Price Estimate** — 1.5 months (15 000$)

**Phase 3** — Release\
**Deliverables** — Shared Memos, Transactions, Notifications\
Once multisig participants are able to send transactions and configure everything from our interface, we plan to implement notifications about transaction requests, incoming and outgoing transactions. Also, we will add a screen where users will be able to track all historical, pending, and partially-signed transactions. Additionally, we want to add a feature of shared transaction memos (stored on IPFS), so that each participant can write and see the same notes related to a transaction.\
**Time and Price Estimate** — 1.5 months (15 000$)

**Phase 4** — Polishing\
**Deliverables** — Design & UX Improvements\
Once everything is set up, we plan to start working with user feedback and analytics, improving our interface according to the user needs. Also, we see a potential need to integrate other smart contract interfaces in our app, i.e. allow users to seamlessly interact with ERC-721 tokens.\
**Time and Price Estimate** — 1.5 months (15 000$)

### Others	 
We are glad to receive your feedback on our beta release of Safari extension
* https://youtu.be/Wk00fIOj2E8 — video
* https://tokenary.io/beta/Tokenary.dmg — download 
