# Alfred Project Plan

The first version of Alfred demonstrates the minimum viable product to gain feedback, show to potential investors, and start early marketing efforts toward potential clients and key influencers. Our goal is to develop and promote protocols that make it safer to self-custody digital assets. With our cryptocurrency inheritance solution, we aim to develop a user base that cares about security and may be interested in purchasing premium services.

## Features
The release offers a simplified product experience that allows users to:

- Plan and manage their estate
  - Create or sync wallets using our web application
  - Deposit and manage funds in an Alfred wallet
  - Define beneficiaries and executors 
  - Issue test requests to simulate the inheritance process

- Generate proof-of-non-activity and proof-of-death
  - Set up 'liveness' monitoring method and parameters
  - Onboard users with KYC if using monitoring that requires collecting PII and transmitting it to a third party
  - Set up third party monitoring, if required
  - Offer payment options and accept payment for premium monitoring services, including recurrent payment processing and handling of payment exceptions   
  
- Access inherited assets

## Other goals
- Integration of the inhertance functionality as a Gnosis Safe app
- Refine the product and pricing strategies
- Refine the marketing and messaging about the product

## System Components


## The workflow of Alfred

### Onboarding
Onboarding is conduct through a dapp. The main objectives are:
1) collect the basic information needed to set up liveliness monitoring and a wallet
2) If LMS is being used, collect payment and perform KYC. KYC is needed to ensure that we are monitoring the liveliness of the right individual and get their permission to do the monitoring. 
3) Configure the oracle contract.
4) Configure the wallet contract.

![Onboarding Flowchart](/Proposals/Alfred/Onboarding.png)

In addition to interacting with the ethereum blockchain, the onboarding dapp interacts with a payment processor, a KYC service, and the liveliness monitoring service.

### Dead Man Switch (DMS) Workflow
![DMS Flowchart](/Proposals/Alfred/DMS.png)

### Live Man Switch (LMS) Workflow
![LMS Flowchart](/Proposals/Alfred/LMS.png)

### Post Death Workflow
![Post Death Flowchart](/Proposals/Alfred/PostDeath.png)
