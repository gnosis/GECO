## Project Overview

### Project name

Defire

[https://defire.io/](https://defire.io/)


### Team members 

Bruno Balzani - https://www.linkedin.com/in/balzani

Daniel Fernández - https://www.linkedin.com/in/dmf7z

### What project are you building 

We are building an SDK  for developers to drive the global adoption of decentralized finance using the full potential of Gnosis' Safe and Modules.

**DEMO VIDEO** on how Defire works on top of Gnosis Safe: [https://youtu.be/vFhwRJtXreg](https://youtu.be/vFhwRJtXreg)

[![Watch the video](https://i.imgur.com/ivO6R6V.jpg)](https://youtu.be/vFhwRJtXreg)

### Why did you decide to build it 

DeFi is expanding rapidly and just starting to redefine the financial system. As more DeFi instruments improve upon the traditional financial system, interest in integration with them will grow. We believe that developers in charge of that integration should not deal with the complexity behind each financial protocol, instead they need secure and tested tools to access them.

### How long will it take 

We estimate 5 months (20-22 weeks) to finish it.

### How much funding are you requesting 
 
We are requesting $52.000.

### How did you hear about the GECO

Manuel García from Protofire told us about it.

## Defire Proposal 

### Project description

Defire enables developers to easily integrate the most popular decentralized finance tools in Ethereum blockchain. It abstracts all the complexity while keeping everything trustless and secure. With a few lines of code a developer can create a Gnosis Safe (portfolio) to hold crypto assets, make payments, lend, borrow, trade and do other financial operations.

Building on top of Gnosis Safe platform, not only provides a secure core for the SDK but the potential to scale it using Gnosis Modules. Every financial instrument that is added to the SDK, is built as a Gnosis Module. Even better, it is possible to provide a granular permission layer to each financial operation. 

### Features


Here is picture of Defire's architecture: 


![Defire's Architecture](https://i.imgur.com/4T8UKYl.jpg)


It consists of different SDKs with actions and queries. An action represents an operation that changes the state of safe. Actions are always decentralized and they involve one or more blockchain transactions. Queries are requests for data or information that can come directly from a node or from Defire's API.


These are the main SDKs: 

**SDK core  (defire-core)**
It provides a way to create Gnosis Safe (portfolios), to add/remove owners (admins), to send ethers or tokens, to enable/disable modules and add/remove operators to those modules. The core SDK is completely decentralized and connects directly to an Ethereum node.

**SDK for modules (defire-compound, defire-uniswap, etc.)**
Each financial instrument is created as a Gnosis Module and has its own SDK. For example, there is a module for Compound (defire-compound), a module for Uniswap (defire-uniswap), etc. It is possible for any developer to create an external module as long as it follows certain rules.

**SDK for API (defire-api)**
The API provides detailed information about the Gnosis safes (portfolios), how many were created, how much they hold (ETH, Tokens, USD amount), who are the owners/modules/operators, financial information like how much has been lent or borrowed, open trading orders, etc. It also gives real time and historical data about each action with its volumes and transactions involved.

It is worth mentioning that all SDKs and documentation are open source.

**Defire Dashboard**
Defire's dashboard provides a UI for any user to view real-time and historical data of each portfolio action, collect metrics and execute some actions directly from it. Some of these actions are creating a portfolio, adding/removing an admin, enabling/disabling a module, adding/removing an operator and giving specific permissions to an operator. The dashboard also help with the user onboarding. 

For more information about Defire SDK please refer to the documentation: https://defire.io/docs#introduction


### Team description

**Bruno Balzani:** Bruno is a serial entrepreneur with a few exit under his belt. He founded FaradayPayments.com, a product for traditional payments that process more than ARS 110 millions each month, that's how he became Official Partner of MercadoPago (the largest Internet payment platform on Latin American). Founder and developer for POAP.xyz (Proof of Attendance Protocol). Also the owner of the first wallet monitor for ethereum: www.etherw.io. He has a bachelor's in Business Administration & Information Systems at Instituto Tecnológico Buenos Aires (ITBA)

**Daniel Fernandez:** Previous: Founder of EasyTrade, the first blockchain aggregator exchange platform with over 1MM USD in trades. Creator of first decentralized exchange for TRON Blockchain. Founder and technical advisor for Ethereum POAP (Proof of Attendance Protocol). Actively involved in crypto space since 2013. Some Accolades: Winner of two Blockchain Global hackathons (DeFi & state channels). External consultant at InGo (USA), Parkio (USA), MeWe (USA). Studies: Software Engineer.

We have known each other for three years. We met in an Ethereum event through a mutual friend and investor. We have worked together at Thoth, looking for trading opportunities using data science and engineering in emerging markets. And recently we have worked on POAP, proof of attendance protocol (https://www.poap.xyz/). A POAP token is a Non Fungible Token that is issued by the Proof of Attendance Protocol following the ERC-721 standard. POAP protocol is doing good, it has been officially used during Devcon5 registration in Osaka, Japan.


### Timeline, Milestones and Deliverables

**Phase I**

Core SDK and API

Deliverables:
> - Smart contract to handle module operators and permissions 
> - SDK to create gnosis safe (portfolio)
> - SDK to add modules to Gnosis Safe
> - SDK to add operators to modules
> - SDK to handle operators' permissions 
> - Service to listen and save gnosis safe and module transactions.
> - API to get account information (actions)
> - API to get portfolio information (actions, modules, operators)
> - Automated tests for core SDK, API and smart contracts.
> - Automated tests for initial API
> - Automated tests for phase I

Time and Price Estimate Delivery: 8 weeks. Funds requested $21000


**Phase II**

Final SDK/API and initial Dashboard 

Deliverables: 

> - SDK that handles payments
> - Module to lend assets (SDK + smart contract)
> - Module to borrow assets  (SDK + smart contract)
> - Module to trade assets  (SDK + smart contract)
> - API to subscribe to action events
> - API to get financial information 
> - Automated tests for final SDK, module SDK and smart contracts.
> - Automated tests for final API
> - Dashboard to connect accounts and portfolio
> - Dashboard to show portfolio's modules

Time and Price Estimate Delivery: 7 weeks. Funds requested $18000

**Phase III**

Final dashboard and complete documentation 

Deliverables: 

> - SDK with third party gas payment (https://gsn.openzeppelin.com/)
> - Dashboard to show portfolio's actions
> - Dashboard to create portfolios
> - Dashboard to manage modules, operators and permissions
> - Documentation for SDK
> - Documentation for API
> - Documentation for Dashboard

Time and Price Estimate Delivery: 5 weeks. Funds requested $13000


### Others	 

We would really love to establish a good relationship with Gnosis team and leverage Gnosis Safe and Modules while driving adoption to the Defi ecosystem.

