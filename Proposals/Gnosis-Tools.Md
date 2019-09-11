# Proposal Guideline 
_This is a guideline on how to best structure your proposal._

## Project Overview

### Project name: Gnosis Tools
--------
### Team members
**Prastut Kumar** - [Github](https://github.com/prastut), [Linkedin](https://www.linkedin.com/in/prastut1/)

**Sahil Nanda** - [Github](https://github.com/sahilnanda1995), [LinkedIn](https://www.linkedin.com/in/sahil-nanda-8b1b88143/)

-------

### What project are you building 
To build an Analytics Dashboard that displays information and various statistics around Gnosis Safe and Gnosis Gas-Station under a single tools website.
### Why did you decide to build it 
We are currently building a [career accelerator](https://www.thevantageproject.com/ICO-blockchain-engineer-hiring/) that upskills experienced full stack engineers with blockchain skills and readies them for remote jobs.

After reaching out to community via Gitter we were pointed to current requirements of the community(thanks to @MareenG) i.e **an analytics dashboard that tracks statistical information around Gnosis Safe wallet usage** and **an interface for a “Gnosis Gas Station” that will display details about Gas price estimates, Gas price calculator, Gas price history, as well as an FAQ**.
Resources:
* https://blog.gnosis.pm/so-you-want-to-build-with-gnosis-but-just-dont-know-exactly-what-c86be7a98314
* https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description-%20Statistics%20Dashboard.pdf
* https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description%20-%20Gnosis%20Gas%20Station.pdf
### How long will it take 
4-6 weeks
### How much funding are you requesting  
10000 USD
### How did you hear about the GECO
[Medium post](https://blog.gnosis.pm/unveiling-the-gnosis-ecosystem-fund-7353926bfb65) by Mareen Gläske from December 2018.

## Your Proposal 
### Project description
_Outline a detailed description of your project, why you chose to build this project, the overall goal and future outlook of your project and why we should fund you._
### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._
#### Individual Component Specs
* Gnosis Safe:
    1. Total Number of Safes Deployed.
    2. Total ETH Stored.
    3. Total ETH Stored in USD.
    4. Total Value stored of other popular Tokens like GNO, DAI and OWL.
    5. An input to check the Amount Stored of a particular token if not listed(that will also guide the user to update the gnosis system if the token is not listed).
    6. Charts:
        1. History of funds stored over time.
        2. Number of Transactions happened over time.
        3. % measure for payment tokens used for transactions over time.
        4. Volume over time for tokens. Initially displaying for popular tokens. Also providing users ability to choose for a particular token.  
* Gnosis Gas Station:
    1. Gas Prices for different Speeds:
        1. Fast
        2. Standard
        3. Safe low
    2. Transaction Fee Calculator:
        1. Inputs:
            1. Gas Used - by the user
            2. Payment Option(Optional) (default ETH) - by the user
            3. Exchange rates- will be fetched automatically and displayed on the screen for the chosen payment option.
        2. Outputs:
            1. Transaction Fee in chosen payment option.
            2. Transaction Fee in USD.
    3. Charts: A price vs time graph for all the three speeds with option to choose start and end date. With on-hover details for a particular time.
### Appendix
#### API Links:
Documenting API links that will be required to display various stats as proposed:
* Number of safes (deployed, not deployed), funds stored(ETH and other supported tokens): https://safe-relay.gnosis.pm/api/v1/stats.
* Funds created over time, number of transactions per day, % of payment tokens used for transactions over time,  Volumes over time: https://safe-relay.gnosis.pm/api/v1/stats/history.
* Tokens Info: https://safe-relay.gnosis.pm/api/v1/tokens/. 
* Payment Tokens: https://safe-relay.gnosis.pm/api/v1/tokens/?gas=true.
* Gas Price Info: https://safe-relay.gnosis.pm/api/v1/gas-station/.
* Gas Price History: https://safe-relay.gnosis.pm/api/v1/gas-station/history.


### Team description
#### Who are we?

Prastut, currently a partner @ The Vantage Project, comes from a UX, product management & full stack background.
Github: https://github.com/prastut 
CV:https://drive.google.com/file/d/15_oS6XtO_DRlITjG6WyTAEavaiSnBsdL/view?usp=sharing. 

Sahil, a software developer @ The Vantage Project will be developing the project full time. 
Github: https://github.com/sahilnanda1995

 

#### Proof of work in other communities:  
- Polkaviz 
    1. Project Link: http://polkavizproject.surge.sh/ 
    1. Community which funded the project: PolkaDAO
    1. Description: a data visualization project of the Polkadot ecosystem. It will start to educate people about the ecosystem and it’s actors. 
    1. Developers: Developed by Sahil, supervised by Prastut. 

- ZCash Health check service status dashboard
    1. Project Link: https://www.zcashservicestatus.info/ 
    1. Proposal Link: https://grants.zfnd.org/proposals/761374418-zcash-service-status-dashboard
    1. Community which funded the project: ZCash
    1. Description: Creating a health check monitoring service for different categories of external services that exist in the ZCash ecosystem. 
    1. Developers: Project supervised by Prastut. 

-------

### Timeline, Milestones and Deliverables
_Detailed description of your timeline milestones and the corresponding payouts_

**Phase I**  			_Outline the different phases_

**Deliverables** 			_What features will be implemented_

**Time and Price Estimate**	_How long will it take and what is the estimated price_

**Phase II**  			_Outline the different phases_

**Deliverables** 			_What features will be implemented_

**Time and Price Estimate**	_How long will it take and what is the estimated price_

**Phase III**  			_..._


### Others	 
Anything else you want to share with us
