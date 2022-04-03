## Project Overview

### Project name
> Minion with Gnosis Safe
### Team members 
> @dekanbro @TomAFrench @wswarren12 @oovg
### What project are you building 
> The purpose of the Safe Minion would be to more tightly integrate The Gnosis Safe into DaoHaus DAOs (MolochV2). This would enable DAOs to have the convenience and familiarity of using the Safe and Safe apps to build transactions, manage tokens and NFTs. It would be a ‘satellite’ account, separate from the main DAO treasury. Essentially the DAO becomes a signer on a Safe.
### Why did you decide to build it 
> Currently creating a minion proposal requires importing abi from somewhere and encoding a transaction. Depending on the size of the transaction this can be very inefficient and gas heavy. Much of this functionality is already created in Gnosis Safe plus other great things like NFT wallets, and wallet connect hookups. Instead of recreating the wheel it would be great to leverage other OSS in the space
### How long will it take 
> 2 weeks
### How much funding are you requesting  
> 3k DAI
### How did you hear about the GECO
> @auryn-macmillan

## Your Proposal 
### Project description
> The Safe minion would be a patern and extension to integrate the Gnosis Safe into MolochV2 and MolochV2x Daos.

> The Minion is a contract that allows the DAO to vote on external contract execution. Here it is used as the glue between a MolochV2 and a Gnosis Safe.

> This setup requires a delegated DAO member to interact with the Safe UI as signer #1. Then 2 minion contracts deployed by the DAO, to act as signer #2 and a backup – an emergency escape hatch if needed. The Safe would be a 2 of 3 setup

> this maybe able to be simplified by using a Gnosis Safe module. Reducing the requirement of having 2 Minions to only 1

### Features
The project will use the Safe api and a front end will be implemented into the Daohaus reactjs front end. We hope that this pattern can be used with other MolochV2 projects and frontends.
The Minion has already been developed and has had a cursory 1 day audit by diligence.
We would like this to work on both mainnet and xdai

#### User Flow: Making proposals
* Delegate builds a transaction in the Safe interface, submits and signs.
* Light DaoHaus UI so delegate can pull the transaction from the Safe api and submit to the Minion. https://github.com/gnosis/safe-contracts/blob/94f9b9083790495f67b661bfa93b06dcba2d3949/contracts/GnosisSafe.sol#L294
* Once minion proposal passes it can be executed (to sign tx)
* Because minion is msg.sender approval is implicit due to the fact that the Minion is the one sending the transaction, transaction executes (gas paid by safe funds or minion), if gas cannot be paid then delegate would need to return to the Safe to execute.

![](https://i.imgur.com/zgJ7dfw.png)

#### User Flow: Meteor strike clause
the dao needs an escape hatch if the delegate goes missing or rouge.

* We need a transaction built that can replace a delegate. 
* Minion 2 submits the replace transaction
* Dao votes, and executes minion when passes (minion or safe needs to pay gas to execute safe tx)
* Dao picks up transaction from api and submits to minion 1.
* Dao votes, and executes minion (minion or safe needs to pay gas here too)
* Using Safe modules we could allow a Minion to call execTransactionFromModule and it would be able to unilaterally swap out a delegate. 

Alternate idea, any dao member can trigger the replace owner tx without a proposal, if it seemed malicious the dao could rage kick the bad member. Could lock funds at least until the kick proposal passes.

If there are no assets in the safe then replacing the delegate is not needed.

![](https://i.imgur.com/NLU7QBP.png)


#### Notes on Setup
1. A delegate sets up the Safe with the two Minion signers or alternatively the Minion module. 


### Team description
@dekanbro - Founder Raidguild and Daohaus, front end developer and project manager.
@TomAFrench - Raidguild member, experience with Safe api, contracts. 
@wswarren12 - Minion proxy factory developer, founder of PoolParty, Lexdao member.
@oovg - Founder Raidguild and Daohaus, Designer and front end developer.

### Timeline, Milestones and Deliverables

**Phase I**  			Research, Spec and Design 

**Deliverables**
* Detailed spec on implementation
* developer engagement and project kickoff
* user flows and ui wireframes
* Frontend design mockups.

**Time and Price Estimate**	4 days 1kDAI

**Phase II** Implementation

**Deliverables** 
* Front end UI
* Api interface
* Gnosis Module development
* Safe contract interface from Frontend

**Time and Price Estimate**	10days 2kdai

### other
Daohaus team will be matching funds
