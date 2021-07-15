# Decentralized spot lending

## Project Overview

### Project name
Decentralized, trustless, p2p spot lending.
### Team members 
Balazs Deme: https://www.linkedin.com/in/balazs-deme-06579450/

Lingraj Mahanand: https://www.linkedin.com/in/lmahanand/

Hilmar Buchholz: https://www.linkedin.com/in/hilmarbuchholz/

Cuong Manh Le: https://github.com/cuonglm

Nicky Gurbani: https://github.com/niktrix

Onuwa Nnachi Isaac: https://github.com/iamonuwa/

Parth Dalal: https://github.com/Parthdalal06
### What project are you building 
We are building a platform where fixed term & interest loans denominated in any cryptocurrency can be drawn and created in a trustless, decentralized manner. Borrowers can request a loan in any crypto, at an interest rate and term they want. There are no collateral requirements as borrowers pick their collateral currency to back the loan including how much of that given asset to deposit. It is up to lenders to pick which loan request to fund by taking into consideration all factors.
### Why did you decide to build it 
Current pooled approaches to facilitate loans in decentralized finance use dynamic interest rates which moves based on supply & demand. This can lead to an unpleasant experience for both lenders and borrowers. On the borrower's side we are tackling two issues: colateral that is dynamically priced & liquidations. Dynamically priced collateral is an issue due to the fact that a current "safe" strategy to draw DeFi loans is to be up to 300% over-collateralized as the price of the collateral can swing dramatically which will lead to it being liquidated. At the same time, liquidations should not be required at all, or in very rare cases while in the current dynamic model big swings can lead to huge collateral being liquidated, further causing a market squeeze. 

On the loan issuers side we create opportunities for fixed term, interest loans rather than the usual 0.x% rates that are common in the DeFi space for mature assets. A big advantage to such an approach is it makes it feasible to create bigger loans without swinging the rates for the whole market. 

### How long will it take 
> 4 months including audit.
### How much funding are you requesting  
> $90,000
### How did you hear about the GECO
On a boat during BBW :-).
## Your Proposal 
### Project description

We admire the way Uniswap exchange is built and would aim to do something of similar beauty and simplicity. This means that loans are created without a central party, through as few, short, secure smart contracts as possible. Our goal is that a loan can be requested or funded through a single contract function which would take requested currency, amoun, collateral type, amount, interest rate requested, duration requested. Loan requests are pooled together in a similar fashion to how order books work, lenders can pick any loan they wish to fund and do so by sending the amount of tokens that are requested. 

There is a web app to everything we outline here in order to provide a smooth experience to everyone, same goes for an easy to use API that aggregates further data from the contracts and makes it easy for anyone to integrate with the protocol and build on it further. Chosing this project for us is easy given our focus on interoperability and briding different blockchains as well as the real-crypto worlds. At completion this protocol will support every asset which Herdius supports which as of today is Bitcoin, Litecoin, Tezos, Binance Coin. At the same time we see a market demand for this product especially from the institutional side, and it would directly compete with centralized providers of fixed term loans. 

Our overall goal is to further the developments, products, reach of DeFi. We think collateralized stablecoins are awesome, but are they really if you need $300 to safely take out a $100 loan? We believe the answer is no, that is why we to make no-collateral loans a possibility in the future. Regarding the funding side, we know how to build all this out and have the experience to do so, but while we focus on interoperability we want to accelerate the development of this exciting product. At the same time we would love to play around where fees go in this product from the sense that ETH fees can be distributed back to GNO holders, etc.  

Future outlook is making this as good of product and baselayer to build upon as possible. Some ideas: integrating on-chain privacy to hide the loans being agreed upon and the amounts, bridging this to the non-crypto world, playing around with locked/staked assets, etc. 

### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._
We plan to use infrastructure and building blocks that are already audited and out there. Reason this is a GECO propoasal is that we will reutilise the Gnosis Safe contracts, because what safer contracts are there to hold funds in? :) The smart contracts will be both in Solidity & Vyper, the APIs we develop will be in Go & Js while the web app is to be done in React. Happy to share architecture layout, and what each contract is going to do in a private email. Of course we would make everything public later on. 
### Team description
We are building Herdius in Go, Js, Angular, Vyper, Solidity so our team covers pretty much anything that is needed to build out a dApp end-to-end. 
### Timeline, Milestones and Deliverables


*Phase I**  			Smart contracts

**Deliverables** 			

Development 6 different smart contracts corresponding to the different fucntionalities of the dApp.


**Time and Price Estimate**	3 months; $48,0000 

*Phase II**  			API & Backend development

**Deliverables** 			

API in Go.
API in Js.
Backend & infrastructure

**Time and Price Estimate**	1 month, $12,000

*Phase III**  			Web App

**Deliverables** 			

Web application in React.
Design of web app.

**Time and Price Estimate**	2 months (runs in parallel), $15,0000

*Phase IV**  			Audit

**Deliverables** 			

Audit report. 
Corresponding changes to Audit if needed.

**Time and Price Estimate**	3 weeks including changes, $15.0000

### Others	 
