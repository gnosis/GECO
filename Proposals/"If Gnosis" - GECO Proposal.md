# "If Gnosis"

## Project Overview

### Project name
> "If Gnosis". The "If This Then That (IFTTT)" for Gnosis.
### Team members 
> Ryan Berkun: https://www.linkedin.com/in/ryan-berkun-47a61a10b/

> Mark Meras: https://www.linkedin.com/in/markmeras/

> Chris Lee: https://www.linkedin.com/in/1smartchris/
### What project are you building 
> "If Gnosis" will launch a protocol-level trigger and events platform for the Gnosis ecosystem. The platform will operate similar to the Zapier (https://zapier.com/) automation platform, with a point-and-click interface, automated API methods, and triggered, cloud based functions.
### Why did you decide to build it 
> Our aim of "If Gnosis" is to further Gnosis adoption by equipping developers with necessary API triggers, such as smart contract events, wallet actions, and market activity, and enriching current Gnosis applications with user-engaging feature sets, such as automated alerts, Conditional Token events, and Google Sheets integrations. 

> While the "If Gnosis" project is innately built for Gnosis developers, the platform's point-and-click solution will be available to all end-users, including token holders, traders, Gnosis Safe users, and user's of Conditional Tokens. 
### How long will it take 
> 20 weeks (5 months).
### How much funding are you requesting  
> $56,500 to build the project to completion.
### How did you hear about the GECO
> Medium post by Mareen Gläske from August 2019.

## Your Proposal 
### Project description
As the cloud platform for blockchain, Fabrx (www.fabrx.io) is a tribe of builders, entrepreneurs, and growth hackers. We envision the digital future to be open to all, and view developers as a key player in driving mainstream adoption of Web3 applications.

With that outlook in mind, we have built the Fabrx platform in order to vastly enhance the developer experience in blockchain. The Fabrx Developer Platform is comprised of many cloud-based functions, including enriched API access layers, point-and-click solutions, cross-chain cloud functions, and automated triggers and analysis.

"If Gnosis" serves as a platform to both (1) simplify the developer experience for new projects and (2) accelerate adoption of current platforms in the Gnosis ecosystem.

These enhanced tools, triggers, and events, will enable new projects to integrate Gnosis functions seamlessly, with minimal code. In addition, by integrating new feature sets into current Gnosis platforms, "If Gnosis" will increase engagement amongst holders, traders, and users within the community.

* Triggers Include: 
    * Wallet actions 
    * GNO / OWL Smart contract events
    * Conditional Token events
    * Gnosis Safe events 
    * Market activity
    
    
* Actions Include:
    * Notifications 
    * JSON response
    * RPC payloads 
    * Conditional Token actions
    * API events 
    * Google sheets actions

We've seen immense demand for the triggers and events platform, both from our close partners and the market (https://twitter.com/corbpage/status/1097237967540674560). We're excited to build out the IFTTT for  Gnosis, and see the platform as a strong opportunity to drive adoption of the Gnosis ecosystem.
### Features
Our goal is to combine the major forces of the Gnosis platform - Prediction Markets and Wallet Custody - into a seamless triggers and events platform. We plan to utilize the Conditional Token, Gnosis Safe, and GNO / OWL contract libraries extensively. 

Phase I of implementation will consist of a full integration of all available API endpoints into a unified Gnosis API. This API will reside at a publicly available endpoint https://GnosisAPI.com (we own the domain). Subsequently, triggers will be integrated from the Gnosis platforms. For example, Conditional Tokens will provide triggers on splitting, merges, and outcomes, Gnosis Safe will provide triggers on safes capabilities (eg. ERC20 fee payment holdings), OpenMarketCap will provide triggers on trading events. Data sources will be integrated based on functionality and demand.

Phase II of implementation will consist of cloud based actions, which developers can plug-and-play into their application. These include email notifications, JSON RPC actions, google sheets data uploads/edits, API actions from the https://GnosisAPI.com public endpoint. Subsequently, trigger and action combinations will be wrapped into API http and websocket endpoints. With the fleshed out trigger and action API, the point-and-click platform will launch, enabling all users to set their own “If, Then” triggers in the Gnosis ecosystem.

**Examples of the "If Gnosis" triggers and actions:**

Conditional Tokens
* Triggers on 
    * Outcome collections
        * If the outcome happens
        * Then do split / merge on another position
    * Splitting and merging positions
        * If other person does split / merge
        * Then do hedge position on ERC20 (eg. GNO)
    * Conditional Resolution
        * If result is X
        * Then send results to database / verify with other oracles

Gnosis Safe
* Triggers on
    * For Individuals
        * Fee payment in ERC20
            * If remaining ERC20 < X
            * Then switch payment to other ERC20 
        * ENS Integration
            * If money sent to ENS
            * Send receipt to Email with ENS address
        * Multiple Safes
            * If portfolio safe > < balance
            * Send notification with rebalance button
    * For Teams
        * Pragmatic multi-sig triggers
            * If one party signs transaction
            * Then send confirmation / notification to other members
        * Fund management (
            * If portfolio trade signal > < X
            * Send notification with rebalance button

__*"If Gnosis" Mockups to Be Attached to Proposal*__

**Userbase for "If Gnosis"**

* Teams
    * Team building platforms on top of conditional tokens (e.g., similar to Veil on Augur)
    * Exchanges to increase market activity through engaging triggers / alerts
    * Wallets to offer prediction markets embedded
    * Current teams utilizing Gnosis Safe, extension to notifications, programatic triggers, database connectors
* Individuals
    * Prediction market users to set conditional triggers
    * Exchange users to monitor and act on on and off chain activity
    * Wallet users to programmatically set global notifications and triggers on changes in their wallet
        * eg. Shortages of coin due to fee paid in ERC20
* Developers
    * Advanced conditional triggers into prediction market with conditional tokens
    * Front-end widget for platforms to seamlessly plug in on-chain and market activity triggers
    * Programable multi-sig trigger / notifications with Gnosis Safe
    * Websocket and API for triggers to be built into backend apps

### Team description
Background:

* Ryan (CEO) built and sold his first startup at the age of 19. In his later years, he went on to launch a handful of projects focused on ML trading applications. In early 2017, he fell down the crypto rabbit hole, and, in mid 2018, left a $2.5M acquisition offer from a Nasdaq company to found Fabrx.
* Mark (CTO) launched a development business at the age of 15. He went on to complete both a bachelor and master degree in Computer Science at Yale, as well as an entrepreneurship focused MBA at the Wharton school of business. Mark has been in the cryptocurrency space since 2013, and founded the Eliza Parker company before leaving to build Fabrx.
* Chris (CMO) founded WiseLee Digital Marketing in 2013, a marketing consultancy that helps local businesses get more customers on the internet. In the following years, he sold his successful e-commerce store and transitioned into the blockchain space in early 2016. Chris assisted in a $20M ICO capital raise in 2017 as Head of PR before leaving to join the Fabrx team.

What we’ve built:

* We are the guys behind Fabrx (www.fabrx.io).
* We have participated in the 0x EAP grant program. Through the program, we launched the ability to deploy a 0x Relayer with one click, as well as a variety of relayer add-ons. Each Relayer is hosted and managed for the end customer, and can be connected to an exchange frontend, “Buy it Now” widget, and market making functionality. To date, 20+ 0x Relayers have been launched through Fabrx on mainnet. This includes live exchanges, such as Merchcoins (https://merchcoins.com/, which has been integrated into Emoon (https://www.emoon.io/), 0xTracker (https://0xtracker.com/)).
* In addition, we are building the Unified Livepeer API: https://github.com/Livepeer-Community-Node/Grant-Program/issues/19.
### Timeline, Milestones and Deliverables
_Detailed description of your timeline milestones and the corresponding payouts_

**Phase I**  			Gnosis Data Driven API & Infrastructure Based Triggers

**1. Data Driven API, Publicly Available at https://GnosisAPI.com**

**Deliverables:**

* Integration of Gnosis infrastructure
    * Gnosis Safe 
      * Data feed
      * Smart contracts
    * Gnosis Conditional Token 
      * Smart contract functions 
      * On-chain contract analysis

* Integration of on-chain activity
    * Etherscan
    * Infura

* Integration of market activity
    * OpenMarketCap
    * Coingecko
    * Exchange data

* Hosting and public availability of https://GnosisAPI.com

**Time and price estimate - 4 weeks, $11,200**

**2. Triggers Based on Gnosis Events**

**Deliverables:**

* Triggers for:
    * Wallet and on-chain transaction events 
    * Smart contract events
    * Conditional token functions and on-chain events
    * Gnosis Safe events in general and specific to deployed wallet
    * Market activity events from market / exchange data

* Hosting architecture for trigger monitoring

* Database infrastructure for triggers enacted and trigger status

**Time and Price Estimate - 6 months, $17,050**

**Phase II**  			Cloud Based Actions &amp; “If Gnosis” Live Platform + API

**1. Cloud-Based Actions, Connected with Triggers**

**Deliverables:**

* Actions for:
    * Notifications for email response 
    * JSON response from smart contract calls
    * RPC payloads from smart contract posts
    * Conditional Token events based on infrastructure
    * API actions from https://GnosisAPI.com
    * Google Sheets actions for upload data

* Hosting architecture for action enactment

* Database infrastructure for actions, as connected with triggers

* API for actions to connect to trggers

**Time and price estimate - 6 weeks, $17,050**

**2. Live Point-and-Click Platform**

**Deliverables:**
* Hosted, full stack trigger-action application at http://dash.fabrx.io
* Front end widget available for use by non-developers
* Front end widget documentation available for platform integration
* Marketplace selection of triggers and actions for non-developers 
* API available for POST requests to subscribe to trigger-action combinations
* Websocket functionality for listening to trigger-action events

**Time and Price Estimate - 4 months, $11,200**


### Others	 
We’ve already started to integrate GNO into the triggers and actions platform:

> Demo of pricing triggers on GNO: https://dash.fabrx.io/thread/pricing/i/alerts/GNO (If GNO price > or < $X)

> Demo of on-chain wallet events on GNO (ERC20): https://dash.fabrx.io/thread/alerts/ETH (If GNO (ERC20) enters or leaves wallet)

General demo of the triggers and actions platform in DeFi:

> Demo in DeFi on Compound: https://dash.fabrx.io/thread/lending/compound/ (If DAI interest rate > X%)
