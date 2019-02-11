## Project Overview

### Project name
> Futarchy Signalling with PM 2.0
### Team members 
John Kelleher - https://www.linkedin.com/in/john-kelleher-86190b/
Mike Calvanese - https://www.linkedin.com/in/michael-calvanese-940b356/
Emily Williams - https://www.linkedin.com/in/ecwilliams66/
Chris Whinfrey - https://www.linkedin.com/in/christopher-whinfrey-5a166783/

### What project are you building 
We are building a futarchy signalling market using Gnosis prediction markets (PM) 2.0, with the idea that they can be used alongside dxDAO decisions.  This is also a step towards allowing voters to delegate votes to futarchy markets in the dxDAO or other DAOs. We will be building on work previously done with Gnosis (https://github.com/levelkdev/fcr-project, https://github.com/levelkdev/fcr-js) and Aragon (https://github.com/aragon/nest/pull/97).

**Futarchy Setup**
Success Metric - This implementation will use Magnolia market cap as the success metric for a decision. An oracle for magnolia's market cap will be developed.

Decision Function - The "decision" will be made based on the outcome that has the higher predicted marketcap for the largest percentage of the decision period.  However, this "decision" will only be for display purposes and will not result in any action while the implementation remains as a signalling market.

Tokenized Event Configuration - For each futarchy decision, a categorical event for the decision being accepted or not accepted will be deployed. The outcome tokens of the categorical event will be used as the collateral tokens for two scalar events that will be used to predict the marketcap given that outcome. For more information on this setup, please see the first configuration described [here.] (https://ethresear.ch/t/possible-futarchy-setups/1820)

LMSR Markets - For each scalar event, an LMSR market will be started for the trading of the scalar event's outcome tokens. LMSR markets require up front funding to ensure a sufficiently liquid market. The burden of funding the market will lie on the user that creates the futarchy decision.


### Why did you decide to build it 
We want to enable DAOs to vote their values and bet their beliefs.


### How long will it take 
3 months

### How much funding are you requesting  
$108,000 USD (cost of 2.5 developers over three months)

### How did you hear about the GECO
Through the Gnosis team.


### Team description
Level K is an established ethereum development company that has been operating since fall of 2017.  We provide blockchain technical architecture, auditing, and development.  We have previously worked on futarchy with Gnosis (presented at DappCon) and Aragon (presented at Aracon).

### Timeline, Milestones and Deliverables

**Phase I**
	Gnosis PM 2.0 Integration

**Deliverables** 
	- Aragon futarchy upgraded to use Gnosis PM 2.0 contracts 
	- Testnet launch of example Aragon DAO

**Time and Price Estimate**	1 month (Feb 18th - March 18th) / 36,000 USD

**Phase II**
	dxDAO Adaptations

**Deliverables**
	- UI improvements for main net launch
	- Upgraded scalar market resolution oracle compatible with dxDAO.  Will likely use market cap of magnolia token as the success metric and DutchX for token information.
	- Implement a way to trigger signalling markets when dxDAO decisions are launched. 

**Time and Price Estimate**	1 month (March 18th - April 18th) / 36,000 USD

**Phase III**
	Main Net Launch of Signaling Market

**Deliverables**
	- Test net launch of signaling market
	- Main net launch of signaling market
	- dxDAO community outreach
	- Blogging and PR to encourage 

**Time and Price Estimate**	1 month (April 18th - May 18th) / 36,000 USD


