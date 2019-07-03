

# SurveyX
Crowd Opinion Mining and Rewarding 
## Project Overview
### Project name
SurveyX

### Team members

_Muhammad Altabba_     - Team Leader

&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/muhammadaltabba/

_Muhammed Mazen Hafez_ - Web/BlockChain Developer


&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/mhmazen/


_Qamar Al-zaman Hafez_  - System Analyst 

&nbsp;&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/qamaral-zamanhafez/

### What project are you building

We are building a survey application that has 2 components:

1) **SurveyX**

A system that facilitates crowd opinion mining and incentivization for any survey that is made for any purpose. This not a prediction market use-case. But, it is a nice example of how some projects could be modeled and built with Gnosis Mercury packages as it is a prediction market use-case. 
 
 2) **NonRepudiationX**
 
 A BlockChain scalability solution that best fit for prediction markets and can leverage Gnosis Mercury and exposes it to more use-cases. In addition to increasing the speed and lowering the cost paid by the end users.


### Why did you decide to build it

We believe that a successful project has to touch the pain of a real business case.

***SurveyX:*** Incentivizing the crowd opinion is the main pain point of any survey maker. So, having a website that facilitates crowd mining and rewarding will solve a real business problem.


***NRX (NonRepudiationX) Scalability Solution:*** BlockChain till now did not reach mass-adoption. And two main reasons for that are the scalability (limited number of transactions per second) and cost (transaction cost is relatively high).

Using _off-chain non-repudiation communication_, that could be claimed on-chain, will enable the users to vote, participate in surveys and do any other activities for free, and they will only pay for the transaction when they will claim their rewards (if there is any).


Actually, we think that SurveyX, like almost all other use-cases that could be built with _Gnosis Prediction Market_, will stay under the hood, if they were not provided with a scalability solution. And we believe that NonRepudiationX is fairly simple, yet powerful enough, and best fit for a prediction market. And it can attract developers and end-users to use Gnosis Prediction Market and the solutions built with.

### How long will it take
The project is estimated to take 6 to 9 months. 

### How much funding are you requesting
56 000 USD.

### How did you hear about the GECO
[Gnosis](https://gnosis.pm/ "Gnosis") website


## Your Proposal

### Project Description

***SurveyX***

Crowd opinion mining and rewarding DApp.


***NRX (NonRepudiationX) Scalability Solution***

BlockChain Off-Chain/On-Chain Scalability Solution.

This scalability solution is based on non-repudiation that can be ensured by the digital signatures which can be signed with Ethereum external-accounts with private/public keys. In this solution, users can participate in a prediction market off-chain. And, the winner can claim his/here reward by posting an on-chain transaction that contains a valid message signed early by the market maker. This will minimize the number of transactions made on Ethereum for any given prediction market. And this will result in 0 participation-cost in any market, in addition to the higher speed. Where the only winner(s) will pay for the fees of the on-chain claim transaction.


### Features

***SurveyX***

This DApp POC is also available at http://surveyx.io. And you can find the source code, and helpful information in the readme file, at https://github.com/apper-tech/surveyx.

Actually, the POC (http://surveyx.io) is built with React, Truffle 5 & and solidity 0.5. However, after getting the grant from Gnosis we will re-implement it utilizing Gnosis Mercury packages; And we will keep it in React.

***NRX (NonRepudiationX) Scalability Solution***

What is non-repudiation? It is the assurance that someone cannot deny the validity of something.  Non-repudiation could be achieved with digital signatures made with the public-key/private-key of Ethereum external accounts (wallets).

The execution flow, that you can see in the next [Sequence Diagram](#nonrepudiationx-sequence-diagram "Sequence Diagram"), is basically that we will ask both the user and the system-owner (the maker or an oracle) to sign, off-chain, their confirmation messages. Such that, the user will first sign his data off-chain.  And then the system-owner, as a confirmation, will off-chain sign the signed message he receives from the user. The user can then use the confirmation he received from the system-owner to claim his reward on-chain. Just like magic, the off-chain signature will be easily done because of the EIP712 standard that is [already implemented in MetaMask](https://medium.com/metamask/eip712-is-coming-what-to-expect-and-how-to-use-it-bb92fd1a7a26 "already implemented in MetaMask"). And thanks to solidity for having [`ecrecover` function](https://solidity.readthedocs.io/en/latest/units-and-global-variables.html#mathematical-and-cryptographic-functions) that can be used for on-chain verification. Additionally, OpenZeppelin provided a standard hash-verification library: https://docs.openzeppelin.org/docs/cryptography_ecdsa.

As a result, this enables the users to participate in any prediction market off-chain. But the one(s) who deserve a reward will be able to claim his/her reward, on-chain. You may find more at https://github.com/apper-tech/nonrepudiationX.



| <a href="#nonrepudiationx-sequence-diagram">![Sequence Diagram of NonRepudiationX](https://github.com/apper-tech/nonrepudiationX/raw/master/nrx-sequence-diagram.png)</a>  |
| :------------: |
|  Sequence Diagram of NonRepudiationX |



## SurveyX POC
- **Main Page**
    
    You will get this page after you launch the app. It is the landing page:
 
<img src="https://drive.google.com/uc?id=1MUi4vwmF4gHE3J6GYiz_7Gibgcmta7qA">

 - **Test-net Main-net Connectivity Check Page**
    
    You might get this page after you launch the app in case of a network misconnection
 
<img src="https://drive.google.com/uc?id=1YbwCsKkfjniGTESPBtnVEQJc9OK2mbR_">

- **Participation Page**
    
    If you are invited to participate in a survey you will see the following screen with appropriate controls to do so  
 
<img src="https://drive.google.com/uc?id=1Zy3bVC7vc1Xh_vHoXHVuRpOUeHEdtM_g">

- **Survey Management Page**
    
    If you created a survey, you can see all the states about it here. Additionally, you will have here an option to end the survey, after enough data has been collected, and a shareable link to the participants
  
 
<img src="https://drive.google.com/uc?id=1iSTgiJEkiITfuxsRaMEMUxnpcHyUgvp1">

- **Survey Creation Page**
    
    A page to create a new survey, define the options, pay the fee and start enrolling participants
  
 
<img src="https://drive.google.com/uc?id=1VHkxBexFbs3CfBqUTZTAgNaZLxafi_mj">

 - **Survey Created**
   
    You will get this page after you create a survey
 
<img src="https://drive.google.com/uc?id=1BwUuMZwwDlu7Dpt7XrrftaQQ_EEVuDYz">

*Kindly pair in mind that the POC (Proof-of-Concept) is an incomplete version that is made only for the purpose of demonstration. And it will be recreated after getting the funds.*


## Team description

***Muhammad Altabba*** 

Full Stack BlockChain Developer with a solid and extensive commercial experience in BlockChain DApps and Web Apps development.

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
		- SurveyX beta version (includes survey builder).
		- Implement NonRepudiationX in SurveyX.
		- Document and encourage using NonRepudiationX for Prediction Markets built with Gnosis.
   - Time and Price Estimate: 2 to 3 months - 18 000 USD



**Phase II:**

Enhancements, Stabilization and Code Refactoring
- Deliverables
    - Heavy testing and bugs fixes.
    - Deploy to Ethereum main net.
    - Implement additional features like reports, a dashboard and etc...
    - Design and implement a business model.
 - Time and Price Estimate: 2 to 3 months - 18 000 USD

**Phase III:** 

Final Technical Touches, Community Building, and Business Model Fine-Tuning.
 
This phase is where we will look more for achievements from a business point of view.

How much effect we could make, is proof of a good technical solution in addition to smart work.

- Deliverables
	- Reach at least 1000 users on SurveyX.io
    - In addition to the above, ensure a successful achievement to at least 3 of the following numbers:
	    - 10 enhancements or feature-requests implementation for opened issues for SurveyX on GitHub.
	    - 1000 viewers for YouTube marketing and/or technical video(s).
	    - 1000 viewers for Medium article(s).
	    - One or more published research paper (most likely about NonRepudationX) in an academic journal or conference.
	    - 1 partnership (at least).
   - Time and Price Estimate: 2 to 3 months - 20 000 USD
   
### What is after those Phases
At the point when we will finish the intended work mentioned previously, we will consider that we had fulfilled our commitment to Gnosis. But will not stop. We will plan for financial stability in addition to new levels of explanation mainly through:
 - Ensuring a revenue stream that keeps the business running and expanding…
 - Continuously look for more partnerships...
 - Raising fund and spending it to gain more market share…
