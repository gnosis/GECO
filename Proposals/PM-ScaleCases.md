# PM-ScaleCases: Scalable Prediction Market Use Cases
 
## Project Overview
### Project name
Prediction Market ScaleCases: InvestorX, SurveyX, and NonRepudiationX (NRX) BlockChain Scalability Solution

### Team members

_Muhammad Altabba_     - CEO

&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/muhammadaltabba/

_Muhammed Mazen Hafez_ - Web/BlockChain Developer


&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/mhmazen/


_Qamar Al-zaman Hafez_  - System Analyst 

&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/qamaral-zamanhafez/

### What project are you building

We are building three components:

1)  **InvestorX**

A prediction market use-case that aims to provide the best financial advice for investors on Ethereum platform. 

2) **SurveyX**

A system that facilitates crowd opinion mining and incentivization for any survey that is made for any purpose. This not a prediction market use-case. But, it is a nice example of how some projects could be modeled and built with Gnosis Apollo packages as it is a prediction market use-case. 
 
 3) **NonRepudiationX**
 
 A BlockChain scalability solution that best fit for prediction market and can leverage Gnosis Apollo and exposes it to more use-cases. In addition to increasing the speed and lowing the cost paid by the end users.


### Why did you decide to build it

We believe that successful projects have to touch the pain of a real business case.

***InvestorX:***
Almost all crypto community are investors who would appreciate good advice and could be engaged relatively easy in investment voting activities. There are already lots of Technical Analysts (on Telegram and specialized sites) with many followers and we will target them all.


***SurveyX:*** Incentivizing the crowd opinion is the main pain point of any survey maker. So, having a website that facilitates crowd mining and rewarding will solve a real business problem.


***NRX (NonRepudiationX) Scalability Solution:*** BlockChain till now is did not reach mass-adoption. And two main reasons for that are the scalability (limited number of transactions per second) and cost (transaction cost is relatively high).

 Using _off-chain non-repudiation communication_, that could be claimed on-chain, will enable the users to vote, participate in surveys and do any other activities for free, and they will only pay for the transaction when they will claim their rewards (if there is any).


Actually, we think that InvestorX and SurveyX, like almost all other use-cases that could be built with _Gnosis Apollo_, will stay under the hood, if there were not be provided with a scalability solution. And we believe that NonRepudiationX is fairly simple, yet powerful enough, and best fit for a prediction market. And it can attract developers and end-users to use Gnosis Apollo and the solutions built with.

### How long will it take
The 3 projects are estimated to take 4 months for core functionality. 

However, because we believe in high-quality and because achieving the business goals will need extra time, we will spend an additional 4 months for things like enhancements, stabilization and code refactoring. And another 4 months for manly for community building and business model fine-tuning in parallel with adding the art-touches on the technical solutions.

### How much funding are you requesting
90 000 USD for working 12 months on the three components: _InvestorX_, _SurveyX_, and _NonRepudiationX (NRX) Scalability Solution_.

Actually, we can have the fund to only one selected item of the above (which is the Scalability Solution). However, we strongly recommend that funding them 3 together. Especially that, InvestorX is built with Angular, SurveyX is built with React and the NRX will expose them, and all other similar cases that can be built with Gnosis Apollo, to mass-adoption.

If you chose to fund only NonRepudiationX, we will need 65 000 USD. This does not mean that InvestorX and SurveyX are very less cheap to implement; But this is because it will be is easier to have a successful business model and/or gather funds to them, away from Gnosis, after their MVP is implemented. However, you may choose to fund NonRepudiationX in this round; And we will apply for InvestorX_, SurveyX in the next funding round after 3 months.

### How did you hear about the GECO
[Gnosis](https://gnosis.pm/ "Gnosis") website


## Your Proposal

### Project Description

***InvestorX***

An Ethereum decentralized application for crypto-investment with decentralized nomination and elections. The DApp aims to elect top investment wallet in term of ROI (return on investment) for a given period.


***SurveyX***

Crowd opinion mining and rewarding DApp.


***NRX (NonRepudiationX) Scalability Solution***

BlockChain Off-Chain/On-Chain Scalability Solution.

This scalability solution is based on non-repudiation that can be ensured by the digital signatures that can be made with Ethereum external-accounts with private/public keys. In this solution, users can participate in a prediction market off-chain. And, the winner can claim his/here reward by posting an on-chain transaction that contains a valid message signed early by the market maker. This will minimize the number of transactions made on Ethereum for any given prediction market. And this will result in 0 participation-cost in any market, in addition to the higher speed. Where the only the winner(s) will pay for the fees of the on-chain claim transaction.


### Features

***InvestorX***

As said, "A picture is worth a thousand words"  and a running prototype worth a thousand pictures. So, we made a POC that you can check at http://investorx.io. And the code is available here https://github.com/apper-tech/investorX and we encourage you to check the readme file as you can find some detailed information there.

Actually, the POC (http://investorx.io) is built with Angular, Truffle 5 & and solidity 0.5. However, after being funded by Gnosis, we will re-implement it utilizing Gnosis Apollo packages. But we will keep it in Angular.

***SurveyX***

This DApp POC is also available at http://surveyx.io. And you can find the source code, and helpful information in the readme file, at https://github.com/apper-tech/investorX.

Actually, the POC (http://surveyx.io) is built with React, Truffle 5 & and solidity 0.5. However, after getting the grant from Gnosis we will re-implement it utilizing Gnosis Apollo packages; And we will keep it in React.

***NRX (NonRepudiationX) Scalability Solution***

What is non-repudiation? It is the assurance that someone cannot deny the validity of something.  Non-repudiation could be achieved with digital signatures made with the public-key/private-key of Ethereum external accounts (wallets).

The execution flow, that you can see in the next [Sequence Diagram](#nonrepudiationx-sequence-diagram "Sequence Diagram"), is basically that we will ask both the user and the system-owner (the maker or an oracle) to sign, off-chain, their confirmation messages. Such that, the user will first sign his data off-chain.  And then the system-owner, as a confirmation, will off-chain sign the signed message he receives from the user. The user can then use the confirmation he received from the system-owner to claim his reward on-chain. Just like magic, the off-chain signature will be easily done because of the EIP712 standard that is [already implemented in MetaMask](https://medium.com/metamask/eip712-is-coming-what-to-expect-and-how-to-use-it-bb92fd1a7a26 "already implemented in MetaMask"). And thanks to solidity for having [`ecrecover` function](https://solidity.readthedocs.io/en/latest/units-and-global-variables.html#mathematical-and-cryptographic-functions) that can be used for on-chain verification. Additionally, OpenZeppelin provided a standard hash-verification library: https://docs.openzeppelin.org/docs/cryptography_ecdsa.

As a result, this enables the users to participate in any prediction market off-chain. But the one(s) who deserve a reward will be able to claim his/her reward, on-chain. You may find more at https://github.com/apper-tech/nonrepudiationX.



| <a href="#nonrepudiationx-sequence-diagram">![Sequence Diagram of NonRepudiationX](https://github.com/apper-tech/nonrepudiationX/raw/master/nrx-sequence-diagram.png)</a>  |
| :------------: |
|  Sequence Diagram of NonRepudiationX |



## Team description

***Muhammad Altabba*** - CEO
Full Stack BlockChain Developer
Solid and extensive commercial experience in BlockChain DApps and Web Apps development.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; LinkedIn: https://www.linkedin.com/in/muhammadaltabba/

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Stack Overflow: https://stackoverflow.com/users/8303489/muhammad-altabba

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Ethereum Stack Exchange: https://ethereum.stackexchange.com/users/23253/muhammad-altabba

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GitHub: https://github.com/Muhammad-Altabba 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Medium BlockChain Articles: https://medium.com/@maltabba

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Google Scholar: https://scholar.google.com/citations?user=sdbpUkYAAAAJ (17 Citations for a bachelor-degree graduation project report that is cited as it is a thesis)

***Muhammed Mazen Hafez***

Experienced Full-Stack Web Developer & BlockChain DApp Developer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; LinkedIn: https://www.linkedin.com/in/mhmazen/

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GitHub: https://github.com/mh-mazen

***Qamar Al-zaman Hafez***

An experienced System Analyst

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; LinkedIn: https://www.linkedin.com/in/qamaral-zamanhafez/

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GitHub: https://github.com/Nayoshca

We will consult and employ many full-time and part-time qualified professionals as needed. But the mentioned above are, the 12 months full-time, dedicated team members who will work hard and smart to turn the ideas to successful projects.


## Timeline, Milestones, and Deliverables
**Phase I:** 
Implementing Core Features
   - Deliverables
		- Rebuild InvestorX and SurveyX with Gnosis Apollo
		- InvestorX beta version
        - SurveyX beta version
        - Create Truffle Boxes (https://truffleframework.com/boxes)
          - Truffle Box for InvestorX as a fully featured sample starting Angular project built with Gnosis Apollo.
          - Truffle Box for SurveyX as a fully featured sample starting React project built with Gnosis Apollo.
          - Creating Truffle boxes means clear and clean code that fit for the purpose, but also generalized for other cases.
        - Implement NonRepudiationX and use it with InvestorX and SurveyX.
   - Time and Price Estimate	4 months - 30 000 USD



**Phase II:**

Enhancements, Stabilization and Code Refactoring
- Deliverables
    - Perform heavy testing and bugs fixes for InvestorX and SurveyX.
    - Deploy InvestorX and SurveyX to Ethereum main net.
    - Integrate NRX with Gnosis Apollo packages (we will fork the repositories and make pull-requests for Gnosis repositories: pm-contracts, pm-js, pm-trading-db and pm-trading-ui).
    - Implement additional app-specific features like pages to view historical data, reports and a dashboard for InvestorX and SurveyX.
    - Design and implement a business model for InvestorX and SurveyX.
- Time and Price Estimate	4 months - 30 000 USD

**Phase III:** 

 Final Technical Touches, Community Building, and Business Model Fine-Tuning.
 
 This phase is where we will look more for achievements from a business point of view. And, this is only doable having a solid and sound solution. So, achieving the deliverables bellow, that could measure how much effect we could make in the market, is a proof of a good technical solution in addition to hard and smart work.
- Deliverables: Ensure a successful achievement to at least 5 of the following numbers:
    - 20 enhancements or feature-requests implemented for opened issues at github.com
    - 2000 users on InvestorX.io and SurveyX.io together (this ensures a good business model in addition to a good technical solution).
    - 2000 viewers for 2 or more Medium articles on how to use Gnosis and Gnosis Apollo (starting from our Truffle Boxes).
    - 2000 viewers for YouTube marketing video(s) that we use to promote InvestorX and SurveyX.
    - 2000 viewers for YouTube video(s) in which we will explain about Gnosis, Gnosis Apollo, including our Truffle Boxes and how to use NonRepudiationX.
    - One or more published research paper (most likely about NonRepudationX) in an academic journal or conference.
    - 2 partnerships with other projects.
- Time and Price Estimate	4 months - 30 000 USD
