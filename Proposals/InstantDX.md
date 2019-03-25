
# Gnosis Grant Application

## Project Overview

### Project name: InstantDX

### Team members
**Hilmar Orth (Hilmar X)** - [Twitter](https://twitter.com/hilmarxo), [Github](https://github.com/hilmarx), [Linkedin](https://www.linkedin.com/in/hilmarx/)

**Luis Schliesske (Bytezantium)** - [Twitter](https://twitter.com/bytezantium), [Github](https://github.com/bytezantium), [LinkedIn](https://www.linkedin.com/in/schliesskeluis/)


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
**Estimated time until completion:**  22 weeks (5.5 months) - Deadline: 23.09.2019

#### How much funding do we need? 
Since we intend to work full-time on InstantDX, the budget for the 5.5 months consists of covering our basic living expenses in Berlin. We estimate those to be $2k before taxes per person per month. Hence the budget for 5.5 months would be $22k (4k per month). Both of us will be working full time throughout the duration of this project phase and would be glad to work at Gnosis HQ in Full Node Berlin, if possible. 

#### How did we hear about the GECO?
[Medium post](https://blog.gnosis.pm/unveiling-the-gnosis-ecosystem-fund-7353926bfb65) by Mareen Gläske from December 2018.


## Proposal

### Project description
#### Why did we choose to build InstantDX?
Upon learning about DutchX, we felt encouraged to take action and do our part in bringing about the removal or alleviation of some of current problems facing decentralized exchanges, which include 1) lack of full end-to-end decentralization in DEX designs, 2) Ethereum’s gas model and fees, 3) lack of adequate liquidity to determine a fair price and 4) DEXs not facilitating smart contracts buying and selling on them. 

#### Why DutchX?
From the stated main problems facing decentralized exchanges today, DutchX sufficiently solves at least the following four of them: 
1. Centralized order books and front-running in current DEX environments
2. Ethereum’s gas fees for cancelled orders.
3. Finding a fair market price for less liquid tokens.
4. Smart-contract enabled trading 

Regarding participation in the DutchX, however, usability constraints undoubtedly emerge for those, who are unwilling to part from liquidity for longer periods of time (~6-12 hours). This concerns any human or smart contract that operates with the need for a continuous flow of liquidity, not just speculators and day-traders. Probably the way people perceive risk in general, and the time-value of money, will urge a significant amount of people to prefer instant order execution over delayed payouts. This hurdle to adoption is exactly what InstantDX aims to remove.

#### A detailed description of the project:
First of all, we would like to make it clear that when we refer to ‘users’, ‘participators’  or ‘sellers’ in what follows, we include both smart contracts and humans in our thinking. Indeed we expect that, sooner or later, a majority of direct traders on the DutchX will likely be smart contracts. 

Gnosis vision is to “build new market mechanisms to enable the distribution of resources—from assets to incentives, and information to ideas”. We share those ideals and want to contribute to the adoption of the mechanisms that will facilitate a fairer distribution of resources across the upcoming global financial crypto economy. 
The goal of InstantDX is add significant value to the DutchX and to greatly accelerate its adoption. To do so, we plan to extend the DutchX suite of features with an option for sellers to bridge the periods of lost liquidity that are an unfortunate byproduct of the workings of this auction mechanism. The time-span of the auctions is forecasted to last 6 hours at a minimum. However, the duration of seller illiquidity could well average on 10 hours, given that sellers cannot submit asks to ongoing auctions, but have to post sell orders beforehand and then wait for the next auction of their trading pair to begin and clear. 
Here, InstantDX significantly adds further value to the DutchX, by providing sellers with instantaneous liquidity via our liquidity pool and payout formulae. It does so by opening the DutchX to humans and smart contracts, who operate and trade with a continuous need for unrestrained liquidity. Examples include: 1) The need to pay for infrastructure fees, 2) apply risk management techniques, 3) interact with  dapps, or 4) the opportunity to earn interest on their tokens.

InstantDX endows sellers on the DutchX with the option to gain instant liquidity from their sell orders. The application achieves this by instantly lending sellers the tokens they want to trade into. InstantDX smart contracts source the tokens to be paid out from a liquidity pool, which in its infancy will be funded from whitelisted addresses. In later stages of the project we will further open the funding of the pool to be permissionless.  Token holders are incentivized to contribute to the InstantDX pool with the opportunity to earn an interest on their stake. Interest payments to liquidity providers are funded by the DutchX-InstantDX users’ interest payments on the instant liquidity they have received. We also intend to source liquidity from lending protocols such as Compound or Maker in future releases.

*Figure 1: InstantDX standard payout mechanism with the following example parameters: previous auction price: 1 ETH = 100 Dai, instant payout rate (‘loan-to-value ratio’) = 67%, auction price: 1 ETH = 100 Dai.*
![InstantDX standard payout mechanism](https://github.com/collateralized/instant-dutchx/blob/master/charts/Instant%20payout%20mechanism%20chart.png "InstantDX standard payout mechanism")


