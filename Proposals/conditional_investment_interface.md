## Project Overview

### Project name
> Simple Conditional Investment Interface
### Team members 
> [David Johnston](https://www.linkedin.com/in/david-johnston-50461b141/)	
### What project are you building 
> Gnosis conditional token based prediction markets have been used to support DAO decision making using [Gnosis Impact](https://impact.gnosis.io/), but ordinary prediction markets are [inefficient](https://forum.gnosis.io/t/change-the-funding-structure-of-gnosis-impact-markets/794/15) for estimating the impact of a proposal. 

> "Conditional investment" is a more efficient market structure for estimating proposal impact. Given a proposal with "yes" and "no" outcomes, a conditional investment market allows people to exchange USDyes for ORGTOKENyes and USDno for ORGTOKENno. The USDyes:ORGTOKENyes market reflects the anticipated value of ORGTOKEN if "yes" is the resolution and the USDno:ORGTOKENno market reflects the anticipated value of ORGTOKEN if the resolution is "no". Unlike standard prediction markets, conditonal investment liquidity providers aren't exposed to large losses if they fail to correctly predict the ultimate outcome when providing their initial investment.
### Why did you decide to build it 
> I am excited to see a world in which conditional investment markets can provide reliable answers to crucial questions and anyone can profit from using their knowledge, skill and judgement to discover answers to these questions. Ethereum is where these ideas are being most actively developed and where, due to DeFi and DAOs, there are potential users interested in experimental decision making technologies and novel financial instruments.

> A simple conditional investment interface may be useful for GnosisDAO to pursue its mission of showing that futarchy can be a high-performance decision making technology, and given my interests it is personally valuable to me to learn about development on Ethereum.
### How long will it take 
> I am a novice at both web development and Ethereum development, and will be working on it part time. I estimate the project will take one month. 
### How much funding are you requesting  
> $750
### How did you hear about the GECO
> GECO grants were explained to me on the GNOSISDAO forum.

## Your Proposal 
### Project description
> The key infrastructure for conditional investment has already been built and deployed to Ethereum mainnet, but but actually making the trades is a deeply convoluted process. I want to build an interface for conditional investment removes two of the biggest obstacles to conditional trades:

 - The need to make transactions on two different interfaces, one for splitting tokens and one for exchaning them
 - The need to manually look up conditional token addresses and import them to the exchange interface

> I believe solving these problems will allow for experimentation with conditional investment with some trading volume, though much more work would be required for a platform intended for general use and large volumes. An experimental platform can be used by GnosisDAO to reintroduce impact estimates to its GIPs in a more cost-efficient manner and to experiment with other ideas related to conditional investment such as creating markets for hyped proposals like EIP 1559 or [measuring the accuracy of impact forecasts](https://docs.google.com/document/d/128PSz7i5JDArrz5EhTeowfzdrlqZPqiyKUP9eLRicwY/edit?usp=sharing))

> GnosisDAO has a commitment to exploring and scaling governance with futarchy, and has an interest in developing a more refined platform for conditional investment. A minimal implementation that can serve as a starting point to identify early adopters and learn about key concerns and issues.

### Features
The conditional investment interface will combine the condition list, split and wrap functions of the [Conditional Token Explorer](https://cte.gnosis.io) with the [Uniswap](https://app.uniswap.org/) exchange interface.

In addition to normal Uniswap interface interactions:
 - Swap page:
	- Select from a list of conditions with readable names
 	- Populate the currency list with collateral and wrapped conditional tokens related to the selected condition
 	- Split collateral against the condition to a default partition with one outcome in each partition
 	- Wrap conditional tokens to ERC20

This will use existing smart contracts - Uniswap Core + Router, Conditional Tokens and ERC1155-ERC20 wrapper. I believe a WIP [updated ERC20 wrapper](https://github.com/gnosis/1155-to-20/tree/feature/support-dynamic-fields) will be needed as currently all wrapped tokens have the same name so users will not easily be able to recognise which tokens they are trading.

### Team description
> > [David Johnston](https://www.linkedin.com/in/david-johnston-50461b141/) ([github](https://github.com/davidoj)) - working on an AI PhD & as a consulting data scientist
### Timeline, Milestones and Deliverables

 - Uniswap trade interface with split & wrap capability
 - Medium article explaining conditional investment & how to do it with splits and trades

### Others	 
