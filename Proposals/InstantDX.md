
# Gnosis Grant Application

## Project Overview
### Project name: [InstantDX](https://github.com/collateralized/instant-dutchx)
--------
### Team members
**Hilmar Orth (Hilmar X)** - [Twitter](https://twitter.com/hilmarxo), [Github](https://github.com/hilmarx), [Linkedin](https://www.linkedin.com/in/hilmarx/)

**Luis Schliesske (Bytezantium)** - [Twitter](https://twitter.com/bytezantium), [Github](https://github.com/bytezantium), [LinkedIn](https://www.linkedin.com/in/schliesskeluis/)

-------
### The Project 

#### Abstract
[Quote](https://blog.gnosis.pm/the-mechanism-design-of-the-gnosis-dutch-exchange-4299a045d523) by Nadja Beneš:
*“The Dutch Auction mechanism is game theoretically known to be an efficient way of determining a fair market price for fungible goods. One drawback of the auction model is that the exchange is not instantaneous (and funds can’t immediately be withdrawn), which makes fast trading impossible.“*

InstantDX is an application built on top of DutchX that will provide an instant payout option to sellers, enabling them to opt out of the various drawbacks associated with having one’s liquidity locked up in long-running DutchX auctions. Instead, they can receive part of their expected payout instantaneously in the form of a bridge loan from the InstantDX liquidity pool. The initial immediate payout is followed by a second payout, after the auction has cleared, to settle the total remaining balance payable to the seller at the actual price that was discovered in the auction.

This will allow users of the DutchX to benefit from all of its benefits, such as fair pricing, gas efficiency, smart-contract enabled trading and the impossibility of front-running, while still being able to perform actions that require an instant exchange of tokens, such as:
- Interacting with dapps
- Paying down large CDPs
- Paying infrastructure fees without the need to hold the network token in large reserves
- Applying certain risk management techniques, to avoid financial losses or make a profit.
- Earning an interest by lending out their liquidity
… and many more.

#### Why did we decide to build InstantDX?
Current decentralized exchanges enable their users to retain true ownership of their assets while trading peer-to-peer in open markets. However, many of the early implementations suffer from flaws concerning their fairness and decentralization in crucial aspects, such as their price discovery mechanism. Gnosis Dutch Exchange offers the first fully decentralized mechanism for finding fair market prices for most crypto assets, especially for those lacking adequate liquidity. In our opinion, being able to always access liquidity at a fair price is essential to create a thriving crypto economy that is not only accessible by the financial and technology savvy, but opens up participation to everyone that wants to be a part of this ecosystem.

However, in order to gain mainstream adoption from both Dapp developers and investors, there needs to be an option to remove the costs of time and illiquidity from the sellers participating in the DutchX mechanism. This is why we think InstantDX can help accelerate the adoption of the DutchX and with it significantly improve the efficiency, fairness and reduce the internal frictions of the Ethereum protocol, in order to fulfil its potential as a global decentralized value transfer protocol.

At the same time, we are very focussed on the possibilities of decentralized lending. Enabling users from all over the world to gain access to cheap capital and move assets from larger investors to smaller ones, allows the creation of wealth to gradually spread more evenly through the ecosystem. Allowing holders of crypto assets to earn an interest on their idle assets is needed to attract more people to switch over to crypto from the old financial institutions, where their dollars in the bank still earn them a ‘risk-free’ interest payment.

We are extremely excited about the improvements the DutchX project and decentralized lending can bring to the current economic systems. We want to contribute to the mainstream adoption of both by providing these synergies to the participants in the ecosystem with continuous liquidity via DutchX-InstantDX. 

#### How long will it take?
22 weeks (5.5 months) - Deadline: 15.10.2019

#### How much funding do we need? 
Since we intend to work full-time on InstantDX, the budget for the 5.5 months consists of covering our basic living expenses in Berlin. We estimate those to be $2k before taxes per person per month. Hence the budget for 5.5 months would be $22k (4k per month). Both of us will be working full time throughout the duration of this project phase and would be glad to work at Gnosis HQ in Full Node Berlin, if possible. 

#### How did we hear about the GECO?
[Medium post](https://blog.gnosis.pm/unveiling-the-gnosis-ecosystem-fund-7353926bfb65) by Mareen Gläske from December 2018.

--------
## Proposal

### Project description
#### Why DutchX?
Upon learning about DutchX, we felt encouraged to take action and do our part in bringing about the removal or alleviation of some of current problems facing decentralized exchanges, which include 1) lack of full end-to-end decentralization in DEX designs, 2) Ethereum’s gas model and fees, 3) lack of adequate liquidity to determine a fair price and 4) DEXs not facilitating smart contracts buying and selling on them. 

From the stated main problems facing decentralized exchanges today, DutchX sufficiently solves at least the following four of them: 
1. Centralized order books and front-running in current DEX environments
2. Ethereum’s gas fees for cancelled orders.
3. Finding a fair market price for less liquid tokens.
4. Smart-contract enabled trading 

Regarding participation in the DutchX, however, usability constraints undoubtedly emerge for those, who are unwilling to part from liquidity for longer periods of time (~6-12 hours). This concerns any human or smart contract that operates with the need for a continuous flow of liquidity, not just speculators and day-traders. Probably the way people perceive risk in general, and the time-value of money, will urge a significant amount of people to prefer instant order execution over delayed payouts. This hurdle to adoption is exactly what InstantDX aims to remove.

#### A detailed description of the project:
First of all, we would like to make it clear that when we refer to ‘users’, ‘participators’  or ‘sellers’ in what follows, we include both smart contracts and humans in our thinking. Indeed we expect that, sooner or later, a majority of direct traders on the DutchX will likely be smart contracts. 

Gnosis vision is to “build new market mechanisms to enable the distribution of resources—from assets to incentives, and information to ideas”. We share those ideals and want to contribute to the adoption of the mechanisms that will facilitate a fairer distribution of resources across the upcoming global financial crypto economy. 

The goal of InstantDX is to improve the user experience of the DutchX and to greatly accelerate its adoption. To do so, we plan to extend the DutchX suite of features with an option for sellers to bridge the periods of lost liquidity that are an unfortunate byproduct of the workings of this auction mechanism. The time-span of the auctions is forecasted to last 6 hours at a minimum. However, the duration of seller illiquidity could well average on 10 hours, given that sellers cannot submit asks to ongoing auctions, but have to post sell orders beforehand and then wait for the next auction of their trading pair to begin and clear. 

Here, InstantDX adds significant value to the DutchX, by providing sellers with instantaneous liquidity via our liquidity pool and payout formulae. It does so by opening the DutchX to users, who operate and trade with a continuous need for unrestrained liquidity. Examples include: 1) The need to pay for infrastructure fees, 2) apply risk management techniques, 3) interact with  dapps, or 4) the opportunity to earn interest on their tokens.

The application achieves the provision of instant liquidity by lending sellers the tokens they want to trade into. InstantDX smart contracts source the tokens to be paid out from a liquidity pool, which in its infancy will be funded from whitelisted addresses. In later stages of the project we will further open the funding of the pool to be permissionless. Token holders are incentivized to contribute to the InstantDX pool with the opportunity to earn an interest on their stake. Interest payments to liquidity providers are funded by the DutchX-InstantDX users’ interest payments on the instant liquidity they have received. We also intend to source liquidity from lending protocols such as Compound or Maker in future releases.

*Figure 1: InstantDX standard payout mechanism with the following example parameters: previous auction price: 1 ETH = 100 Dai, instant payout rate (‘loan-to-value ratio’) = 67%, auction price: 1 ETH = 100 Dai.*
![InstantDX standard payout mechanism](https://github.com/collateralized/instant-dutchx/blob/master/charts/InstantDX-payout-%20mechanism-%20chart.png "InstantDX standard payout mechanism")

In essence, the application offers DutchX users a new choice in their interactions with the exchange. If instant liquidity and time is not of interest to the seller, they can proceed with the normal auction process. However, if liquidity and time is of importance, as will be the case for many humans and automata, they can gain value from InstantDX in the normal scenario like so:

#### Payout Formula: 

_Note: The payout formula is written from the perspective of the InstantDX liquidity pool_

**Payable1ToUser** = P0 * Q * LVR

**AuctionReceivable** = P1 * Q 

**Payable2ToUser** = AuctionReceivable - Payable1ToUser  - interest

--------

**Where:** 

**P0** is price of previous auction 

**P1** price of upcoming auction, 

**Q** is quantity sold by the seller, 

**LVR** is the loan-to-value ratio ,

**interest** is the interest paid to the pool.

*Figure 2: InstantDX vs. regular DutchX payout process*
![InstantDX vs. regular DutchX payout process chart](https://github.com/collateralized/instant-dutchx/blob/master/charts/InstantDX-vs-DX-payouts-chart.png "InstantDX vs. regular DutchX payout process")

1. A seller wants to sell a certain quantity _**(Q)**_ of a token on the DutchX using InstantDX and sends the tokens to our smart contract.
2. The smart contract places the sell order on the DutchX
3. The InstantDX pool immediately transfers a bridge loan _**(Payable1ToUser)**_, meaning _**Q * LVR (e.g. ~67%)**_ of expected tokens, to the seller using the previous auction price _**(P0)**_ as a benchmark. 
4. The auction settles on a price _**(P1)**_ and clears the total sell volume _**(Q)**_. The purchased tokens _**(AuctionReceivable)**_ are transferred from the DutchX to InstantDX’s smart contracts
5. InstantDX smart contracts pay out the outstanding trade balance _**(Payable2ToUser)**_ to the seller.
6. The interest paid by the seller gets distributed among InstantDXs liquidity providers

In order to protect the liquidity providers of the InstantDX pool against possible black swan events, in which the auction settles on a price for the receivable token that is less than the 1 - LVR safety margin, we introduce three safety mechanisms:

1) For every sale through InstantDX, 10% of the pools earned interest is accumulated within the pools buffer. Those funds will be used to compensate potential losses of the overall pool.
2) Similar to other lending protocols, in our early versions we will only include low risk collateral tokens combined with low LVRs. We intend to gradually introduce more token pairings as the volatility of these assets decreases over time. 
Only in an extreme edge case where these two safety mechanisms fail, the pool automatically conducts safety mechanism number three:
3) Haircutting the entire pools liquidity by the incurred losses. 

We are convinced that despite the aforementioned risk, liquidity providers will still be strongly incentivized to contribute funds to the InstantDX pool. They will be compensated for the minor risk they incur, by having significantly more interest accrue to them compared to that of other lending protocols, like Compound, which aim to be the risk-free rate of the market. This is possible because, even though interest paid by individual sellers participating in the DutchX-InstantDX will be very small, these isolated marginal payments are compensated for in the high sell volumes to be expected on the DutchX. In fact, the interest earned by liquidity providers will accumulate every 6 hours on average.


#### Overall goal and future outlook:

#### Overall goal
The overall goal of the project is to build and seamlessly integrate a first version of InstantDX with the DutchX protocol, in order to enable sellers to be able to receive instant payouts on their DutchX sell orders. Our target users are developers, smart contracts and sophisticated end users that want to provide themselves, or their users, with access to the DutchX auction mechanism and its promise of fair pricing, whilst still having access to instant liquidity, thanks to InstantDX’s real-time payout feature.

#### Future Outlook
After enabling the InstantDX application for the first trading pair, other crypto assets can gradually be added to the offering. Beyond that, the system can offer a variety of additional features to the DutchX users, such as:
1. Automated price insurance, which guarantees the seller a minimum ask price for their sell order by automatically placing a buy order in the auction at a minimum ask price they can specify.
2. Automated lending of sellers’ liquidity on lending platforms, to have instant interest accrue to them.
3. Integrations of InstantDX with other applications, like dapps built on top of MakerDAO that manage CDPs, by enabling them to automatically purchase large sums of Dai on the DutchX instantaneously,  in order to avoid liquidation of their CDPs
4. Usage in prediction markets, such as Gnosis, to provide instant liquidity for certain types of bets when the outcome can be predicted with high probability, similar to the “cash out” service of modern sport betting companies.

-------
### Features

#### How do we plan to implement InstantDX?
*Figure 3: Smart Contract Architecture*
![Smart Contract Architecture diagram](https://github.com/collateralized/instant-dutchx/blob/master/charts/InstantDX-smart-contract-architecture.png "InstantDX Smart Contract Architecture")

*Note: Version 0.1 of the InstantDX app comprises parts 1 & 2. Part 3 will be part of the next iteration:*

#### Part 1: Creating an escrow contract that interacts with the DutchX
The escrow smart contracts objective is to act as the address that sells and collects the users tokens to and from the DutchX. For each sell order, a unique escrow contract will be deployed by the respective pool contract. The escrow contract provides 4 core functionalities: 
1) Accepting funds from the pool contract.
2) Selling the received tokens on the DutchX.
3) Claiming the funds receivable upon settlement of the auction.
4) Transfering the received tokens to the pool contract. 

#### Part 2: Pooling collateral from investors and creating a micro lending platform
The counterpart of the escrow contract is the pool contract. Its purpose is to pool funds from individual contributors, calculate and facilitate the payouts to sellers, and transfer the earned interest to the liquidity providers of the pool. There will be an individual pool contract for each ERC20 token locked in the InstantDX system with customized LVR and interest fees. Each of these pools contain a ledger of all transactions to borrowers and liquidity providers. 

#### The core functionalities of the Pool Contract are:
1) Verifying that sufficient funds are present to cover the initial instant payout.
2) Accepting seller tokens, if sufficient funds are present.
3) Deploying an individual escrow contract.
4) Paying out the first payout (bridge loan) to the seller.
5) Receiving tokens after auction settlement from escrow contract.
6) Transfering the second payment to the seller after the auction ends.
7) Distributing interest among liquidity providers.
8) Building up an internal liquidity buffer to defend against possible black swan events.
9) Accepting withdrawals and transferring requested funds back to liquidity providers.

We are aware that, at start, it requires some additional funding to initialize the liquidity pool. However, by restricting the total sell volume to be handled by InstantDX at any given time, and by limiting the supported token pairs we can gauge the required up-front capital and set it to a manageable amount, in order to scale the project in a controlled fashion. 

At the beginning the list of possible investors to the pool will be whitelisted, meaning that before accepting permissionless third-party money, the contracts will have to be tested rigorously on mainnet and with selected investors that accept the risk of losing funds.

#### Part 3: Connecting InstantDX to other lending platforms to access an even larger pool of liquidity 
The beauty of a permissionless blockchain protocol like Ethereum is that we can tap into the liquidity of other already established lending platforms such as Maker or Compound, in order to increase InstantDXs ability to provide instant liquidity to even more DutchX users. This will be achieved by a third major contract called Platform Manager, which serves the following functionalities:
1) Comparing interest rates and maximum borrow amount on pre-selected lending protocols, in order to select the most economical option.
2) Depositing collateral at chosen lending protocol.
3) Borrowing the required asset being purchased by the DutchX seller.
4) Transferring the funds to the Pool Contract.
5) Receiving the acquired tokens after dutch auction has been settled from the Pool Contract.
6) Wiping the loans debt.
7) Sending the freed up collateral back to the Pool Contract.

The platform manager contract will be customized for each lending protocol and autonomously manages the credit positions of the liquidity pool. At first we will most likely only use stable DAI as collateral for acquiring loans on these platforms, in order to mitigate collateral liquidation risks. As soon as more complex derivatives gain the necessary liquidity on Ethereum, such collateral types can be used, and their risk can be managed accordingly by the Platform Manager smart contracts. 

#### Tools and frameworks:
- Smart contracts: Solidity
- Documentation: Web3, Javascript
- Testing & Deployment: Truffle
- Libraries: SafeMath.sol, SafeToken.sol

------
### Team description
#### Who are we?
Luis & Hilmar have been working together on projects since 2016, founded two companies along the way and led software development projects using Ethereum for multiple Fortune500 companies. 
#### Hilmar Orth aka HilmarX
- Full Stack Developer (Solidity, Javascript, Python, C, Ruby)
- Hooked on DAOs - first ever [tweet](https://twitter.com/hilmarxo/status/735567875793137664) was about “The DAO” 
- Co-founded and led energy blockchain startup DEEP (d33p.org)
- Participant of ETHSingapore & Prize Winner at ETHParis 

#### Luis Schliesske aka Bytezantium
- Full Stack Developer (Python, Solidity, C, JavaScript)
- Political Economy graduate at King's College London
- Enjoys to theorize about games
- Co-Founded and headed Konfid.io Contract Solutions. Led project developing private blockchain MVP at European Fortune100 company.

#### Latest collaborative Projects: 
- [Collateralized](https://github.com/hilmarx/collateralized) - Decentralized Interest Rate Swaps on Ethereum. Allows borrowers and lenders to refinance their loans between multiple lending platforms like Maker and ETHLend.

- [IPFSWAP](https://github.com/hilmarx/ipfswap) - Enables ERC20 token swaps using Kyber Networks liquidity hosted on IPFS.

-------
### Timeline, Milestones and Deliverables

#### Overall Deliverables:

The overall goal will be the deployment of InstantDXs v0.1.0 on Ethereum mainnet, in order to test our idea out in the wild with a preselected set of liquidity contributors. Version 0.1.0 encompasses the aforementioned steps 1 & 2 plus the creation of developer documentation. Step 3 would be a natural next step after this phase to increase the number of token pairs supported by InstantDX.
In the scope of the project, the more specific deliverables are:
1) Development and deployment of Escrow and Pool smart contracts facilitating the escrow, token transfers, pooling, borrowing, interest payment, lending and fee calculation operations 
2) Creation of developer documentation outlining how to integrate the InstantDX feature in user facing applications like slow.trade and other developer targeted applications
3) Creation of a liquidity pool of at least one asset (e.g. DAI) that can kickstart the liquidity provision.

#### Detailed description of your timeline milestones and the corresponding payouts
#### Phase I - Development of Escrow.sol + deployment & testing on Rinkeby
**Goal:**

Deployment of escrow contracts to act as a secure interface between a simulated future pool contract and the DutchX.

**Deliverables:**
- Development Escrow.sol
- Deployment Rinkeby
- Unit & integration testing
- Gas optimization

**Time and Price Estimate**
- **Time:** 1.5 months
- **Deadline:** 15.06.2019
- **Price Estimate:** 6k 

#### Phase II Development of DaiPool.sol + deployment & testing on Rinkeby
**Goal:**

Deployment of pool contract, accepting e.g. Dai as collateral, interacting directly with  deployed escrow contracts and transfering funds to the seller.

**Deliverables**
- Development DaiPool.sol
- Price oracle selection and integration
- Deployment Rinkeby
- Unit & integration testing
- Gas optimization

**Time and Price Estimate**
- **Time:** 2.5 months
- **Deadline:** 30.08.2019
- **Price Estimate:** 10k 

#### Phase III Iterations on both Escrow and Pool Contracts & mainnet deployment of  v0.1.0 + seeding of pool
**Goal:**

Successful completion of test phase on Rinkeby and mainnet deployment

**Deliverables**
- Mainnet deployment of InstantDX v0.1.0
- Pool seeding and beta testing with whitelist investors
- Creation of developer documentation

**Time and Price Estimate**
- **Time:** 1.5 months
- **Deadline:** 15.10.2019
- **Price Estimate:** 6k 

### Remarks
Our team will be working full time on this project and plans to continue its implementation beyond the scope of this grant. 
The other passion our team shares with Gnosis is decentralized governance. Our long term plan would be to create a - or integrate with an existing - DAO which manages the risk parameters of InstantDXs lending activities and makes crowdsourced decisions about what application to integrate next. We would be thrilled to gain & share insights regarding such opportunities from the Gnosis team and start a discussion about how the dxDAO could be a part of that.

