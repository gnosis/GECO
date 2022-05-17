# Proposal Guideline 

## Project Overview

### Project name
Universal Login

### Team members 
* Alex Van de Sande
* Marek Kirejczyk


### What project are you building 
We are building tools for developers to help them onboard their users faster, easier and with as fewer dropoffs as possible.
Currently, we built our own gasless, ens creating, meta-transaction enabled, smart contract wallet, but we would like to migrate to Gnosis Safe. We want to make Gnosis Safe a part of a full onboarding solution for new users.

### Why did you decide to build it 
We understand that allowing users to pay for transactions or deployment of the contract is a real game-changer. We built a system that counterfactually deploys a wallet, integrates with multiple on-ramping provider in many countries, and automatically register an ENS name for the end-user. The signup can take less than 2 minutes (depending mostly on the onramp provider). We built it and launched from scratch, mostly because when we started Gnosis Safe was still under development. 

But now as many projects mature we are taking a deeper look on building on top of other mature projects and gnosis safe is a great alternative. 

### How long will it take 
We estimate 8-12 weeks to complete the full transition.

### How much funding are you requesting  
US$25,000.00

### How did you hear about the GECO
We follow Gnosis developments closely and been to multiple Dappcons.


## Your Proposal 
### Project description
We plan to migrate completely our SDK to Gnosis Safe. That would include a system that: allow users to log into apps by picking an ENS username, deploying a contract and registering a new ENS name when it doesn't exist and managing and registering new private keys when the account already exists.


### Features
1) ENS signup attached to wallet creation, so that the user has a name the minute the wallet is created 
2) Integrated on-ramping providers from multiple countries
3) SDK for easy app development that would use Gnosis safe as the main identity account
4) Relayer that accepts transactions paid in tokens 

### Team description
Marek and Alex met at a DappCon, invited by Gnosis to talk about the concept of Universal Login. Alex has been working with the Ethereum foundation with onboarding since 2014. Marek has built many internet companies and founded EthWorks. 
Universal Logins is now an independent company incorporated in the US and seeking all investment opportunities to help us realize our vision of better onboarding for ethereum apps.


### Timeline, Milestones and Deliverables

We intend to release in two phases:

**Phase 1: (4-6 weeks)** 
*US$10,000.00*

- integrate with existing Relayer & SDK

**Phase 2: (4-6 weeks)**
*US$15,000.00*

1. Add ENS name functionality to smart contracts
2. Add new Gnosis Safe functionality to Universal login: 
- multi transactions
- daily limit

### Others   

This grant is not a requirement for us to use Gnosis safe, we are looking into it and are considering adding to our flow. But grant approval would be a very positive signal for us, and would certainly allow us more flexibility to integrate more tools of safe into Universal Login.



