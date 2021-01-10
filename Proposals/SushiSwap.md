## Project Overview

### Project name
Safe Sushi Swap
### Team members 
Max Fritz [GitHub](https://github.com/fritzschoff)
### What project are you building 
I'm building an interface for the Sushi Swap App.
### Why did you decide to build it 
Sushi Swap already offers a lot of features which would enrich the gnosis safe app ecosystem. 
### How long will it take 
More then 10 Days.
### How much funding are you requesting  
High complexity => 3000$ + 3000 from Sushi Swap - [Link](https://blog.gnosis.pm/introducing-the-gnosis-safe-sushiswap-grant-f2e597c6d6cb)
### How did you hear about the GECO
Rafael Suarez told be about it.

## Your Proposal 
### Project description
I'm going to implement the possibility to interact with the Sushi Swap DEX with all the features of what the exchange feature from Sushi Swap offers.
- Set limit order.
- Set market order.
### Features
### Team description
It's only me.
### Timeline, Milestones and Deliverables

**Phase I**  			

**Deliverables**    In the first phase I will implement the market order feature from Sushi Swap. The interface will apply the gnosis safe app UI [guidelines](https://drive.google.com/file/d/18QxvqPzJ39Da3peSId0hJe9dL2mSB818/view). 
You are going to have two inputs with an autocompletion of the available tokens. Also by just pasting the address of a token into the input, it will generate a token out of the address and fetch all the possible information that are available.
After the first token has been chosen, it will check for the allowance and will ask the user to approve the token.
In this phase I will also need to write all the necessary unit and e2e tests.

**Time and Price Estimate**	This will take about 8 days. 50% payout of the grant.

**Phase II**  			

**Deliverables** 			In the second phase I will add the feature of setting a limit order. This would add two buttons on the top of the app where you can toggle between market and limit order. In the limit order section, there are going to be another two inputs below of the chosen tokens that are going to be swapped and what the expected return is going to be. 
I also need to implement a dashboard where you successful, canceled or pending orders are visible. Also you should be able to cancel pending limit orders.

**Time and Price Estimate**	5-8 days. Rest of the grant.


**Phase III**  			

**Deliverables** 		This phase is on going since the limit order feature of sushi swap is currently in beta and so the safe sushi swap interface needs to be maintained.
In this phase, it would be also possible to add the[ Gelato Network](https://github.com/gelatodigital/gelato-network) to this interface. This would allow the feature of pending limit orders that never expire and also set up an order on arbitrary conditions.

**Time and Price Estimate**	...?
