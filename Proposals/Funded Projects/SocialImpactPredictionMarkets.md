## Project Overview

### Project name
Social Impact Prediction Markets

### Team members 
[Raphaël Mazet](https://www.linkedin.com/in/rapha%C3%ABl-mazet-5b76721/) - Project Management

[Jakub Wojciechowski](https://www.linkedin.com/in/jakub-wojciechowski-5901b68/) - Blockchain dev / Tech lead

[Alex Suvorov](https://www.linkedin.com/in/alex-suvorov-40528b158/) - Full-stack dev

[Areti Kampyli](https://www.linkedin.com/in/aretikampyli/) - Ux design

[Dhen Padilla](https://www.linkedin.com/in/dhenpadilla/) - Front-end dev

### The project we’re building
 
Since 2015, the Alice team has been building a transparent social impact platform on Ethereum. The core mechanism is a “donation by results” mechanism whereby nonprofits only receive donations once they prove that they’ve achieved their goals. This proof is verified by an independent validator (human or machine), aka an impact oracle. This dApp has been live since 2017, with 3 pilots run to date, and another 10 due to be launched this year.

Last year, we started working on a complementary impact investment platform, which allows investors to provide upfront seed capital to NGOs so that they can start projects (as NGOs only get donations after achieving their goals). Investors underwrite the risk of projects failing, but they also get paid back automatically and with interest, from the donations, as and when outcomes are achieved.

In our system, impact investors receive what we call “coupon tokens” in exchange for their investment. In effect, these are conditional tokens that give them a right to be paid back from escrowed donations.

The aim of this grant application is to refactor our code so that we use the Gnosis conditional tokens instead of our existing implementation. We expect that this will improve usability, increase liquidity, and allow for project signalling, far beyond what we could achieve if we rolled our own conditional token system.

### Why we decided to build it
Impact investing has been on our roadmap from the start, and our system is inspired by an existing impact investing asset class called social impact bonds (SIBs), where the outcome payer is generally the government, rather than individual donors on Alice. Alice is essentially creating a platform for decentralised impact bonds with the following benefits:

  * **Tradeable**: currently, governmental SIBs are bonds only in name. They cannot be traded, and certainly cannot benefit from the advantages of a prediction market

  * **Scaleable**: SIBs are temporary contracts that end when all funds set aside by the outcome payer (generally the government) have been exhausted. Alice allows for a perpetual funding model, where NGOs can keep raising donations and impact investment as long as they can demonstrate their impact.

  * **Transparent**: the contractual terms of government-backed SIBs are opaque, as is the track record of the NGOs that are funded by them. Alice provides full transparency on both these fronts.
  
Overall, our ambition is to completely transform how social impact is funded, with full transparency that allows funders to discover the most effective social and environmental projects, and help them scale rapidly. 

### Expected timeline 
We expect this project to take 8 months to complete.

### Funding request
  
$25,000 (Phase I - core impact investing tokens) + $25,000 (Phase II - Signalling)

### How we heard about the GECO

A presentation at EthCC in Paris.

## Our Proposal 
### Project description

In the Alice ecosystem, there are two types of nonprofit funders:

  * **Donors**: these funders make philanthropic gifts to social and environmental projects. These gifts are conditional however, and are held in escrow in a smart contract until the nonprofit running a project proves that it has achieved its predefined goals (e.g. helping a homeless person find long term accommodation).
  
  * **Impact investors**: these funders provide upfront money to nonprofits, so that they have the resources to start a project. Crucially, the nonprofit is not directly liable to pay back investors. Instead, investors are repaid from escrowed donations, as and when the nonprofit achieves its goals. In effect, these investments are collateralized loans, repaid automatically on the condition that the nonprofit’s goals are achieved.

*This proposal will focus on Alice’s impact investment protocol, not on the donation side.*
 
In the first implementation of Alice’s impact investment process, investors received “coupon tokens” in exchange for their investment, with new tokens minted each time an investment was made. These followed the ERC20 standard, and were meant to be tradeable in our future roadmap. A demo of the process can be found [here](http://demo.alice.si/), and the code base [here](https://github.com/alice-si/contracts).

With this GECO grant, we propose to refactor the Alice code base to substitute our coupon tokens with Gnosis conditional tokens, that will give investors a much richer set of options than currently available.

#### I. Base implementation of conditional social impact tokens in the core Alice impact investment protocol
 
Gnosis [conditional tokens](https://gnosis-mercury.readthedocs.io/en/latest/index.html) from the [Mercury](https://github.com/gnosis/hg-contracts/blob/master/contracts/PredictionMarketSystem.sol) release are a very interesting abstraction to implement the investment flow in Alice, given that each investment is in effect a collateralized loan, which is only repaid on the condition that social projects achieve their goals. Our implementation of the Gnosis conditional tokens will be called conditional social impact tokens throughout this proposal, and the protocol will be implemented as follows:

1. A nonprofit creates a new social project on Alice. It specifies the goals it is aiming to achieve, and the amount that will be paid for the completion of each goal

2. Donors make donations to a specific project. These funds are held in escrow in a project wallet.

3. Impact investors make loans to the social projects, so that the nonprofit running it can start the work needed to achieve its goals. In exchange for their investments, investors receive conditional social impact tokens.

4. Once a goal is achieved, the nonprofit makes a claim and provides the proof of its achievement to an independent validator (aka an impact oracle), tasked with verifying that the claim is correct.

5. This validator effectively acts as an oracle for the contract, and if a claim is accepted, it triggers two transactions: part of the escrowed donations are paid directly to the nonprofit, and part is allocated to pay back investors, at which time part of their conditional social impact tokens are burnt.

The following diagram shows a high-level technical architecure of the Social Impact Investment platfrom: 

<p align="center">
  <img src="https://github.com/alice-si/GECO/blob/master/Proposals/assets/SocialImpact.png" />
</p>


#### II. New hedging and signalling mechanisms enabled by the use of the Gnosis protocol

The new version of the Gnosis [prediction markets](https://blog.gnosis.pm/prediction-markets-2-0-teaser-4ee1cfa3d61f) contracts provides very powerful features that can be used in the Alice protocol for hedging and signalling purposes.
This is because of the way that social projects are structured on Alice, with multiple goals, that can be parsed as conditions in a Gnosis framework.
 
For example, a social project that aims to help people on the brink of homelessness by helping them find a job may be structured as a sequence of goals:
1. a person in need is referred to the program and is assigned a key worker,
2. interview and job training starts,
3. the person graduates from training,
4. the nonprofit helps the person secure an internship, and then finally
5. a permanent job. Each of these milestones may be verified by an impact oracle and trigger payments in the Alice protocol.

#### 1. Hedging

Implementing every milestone as a separate condition will offer a fine-grained project structure that could be used for more accurate signalling or well-tailored investments. 

We will use this grant to develop three distinct hedging mechanisms using prediction  markets enabled by the use of conditional social impact tokens:
 
  * The first and simplest will simply allow impact investors who have provided money upfront to nonprofits to take the opposite position on a prediction, hence ensuring that they do not lose their entire investment if the project fails.
  
  * The second hedging mechanism will allow impact investors  to split the various “conditions” of their token, and trade them on. This would allow complex social projects (e.g. a project providing mental health support and job training) to be split into component parts, and allow investors to only keep outcomes that they are interested in (e.g. an investor may only care about the mental health support and not the rest).
  
  * Finally, conditional tokens will allow investors to hedge their risks against external factors. For example, an investor in a job training project may consider that Brexit could lead to higher unemployment rates hence making it significantly more difficult for the nonprofit to achieve its goals. In this case, the investor could split the tokens on the condition of Brexit happening and sell on that risk to a third party who would be willing to accept the higher risk exposure in return for higher potential returns.

#### 2. Signalling
 
The use of a prediction market based on each project’s conditional social impact token will allow for precise market signals and potentially integrate the voice of people being supported by projects directly.
 
  * **Precise signalling**: splitting and merging conditions (each project’s specific goals) will allow the markets to help guide investment decisions and even provide operational suggestions to nonprofits. For example, if the markets believe that a key part of the program, such as the process for finding internships, is flawed, it can bet against the achievement of this goal while support all previous conditions.
 
  * **Beneficiary signalling**: we would like to use this grant to implement a specific kind of signalling provided by the beneficiaries of a project themselves. To do so, we would airdrop conditional social impact tokens on beneficiaries to allow them to weigh in on whether they believe that the social project is well adapted to their needs or not. This could obviously lead to skewed incentives and attack vectors, and part of the grant will be used to explore these and mitigation tactics.



### Features

#### Phase I: Social impact investing protocol

1. **Integration of conditional tokens in the core Alice protocol**

We will refactor our social impact investment [contracts](https://github.com/alice-si/contracts) to utilise the [conditional tokens](https://gnosis-mercury.readthedocs.io/en/latest/index.html) from the Gnosis Mercury release as a base component of our conditional social impact token (previously known as the “coupon token” as explained above). This will provide the required flexibility of token splitting and trading and avoid the use of more complex external contracts.

As the conditional tokens are still a relatively new concept, the integration will involve in-depth testing of the new approach, internal security audits and attempts to optimise the gas consumption. We will also explore the possibility of splitting multiple collaterals and provide a full implementation of position transfer/trading features interfaced by the [ERC-1135](https://github.com/enjin/erc-1155/blob/master/contracts/ERC1155.sol) base contract. We would like to pioneer the new set of use cases for the conditional tokens to be seen as generic building blocks for investment contracts.

2. **Simple UI for bonds creation, trading & splitting**

Impact investors should be able to easily split and merge the conditional tokens to improve their flexibility of risk handling. We are going to implement a simple UI based on a dapp architecture that will allow defining the conditions for a split, connecting to external oracles and merging the previously split tokens. 

The interface will consist of a view that will display a list of conditional tokens currently held by investors. There will be also a detailed view per every token that will show the conditions and connected oracle. Users will have the ability to propose splits and provide the oracle details.

3. **Regulated trading-splitting controllers**

A token representing social impact is a financial product that could be classified as a security. Therefore there is a need to implement restrictions that will govern how the tokens are distributed and traded. Currently, we’re working with two international law firms on the specification for blockchain based social impact investment tokens to assure that they are fully compliant with the financial regulations.

We plan to implement a controller contract that will contain all of the regulatory imposed limitations. The controller contract will act as a wrapper around a conditional token that will mediate the transfer methods. There will be a way to exchange the controller if tokens need to be adapted to another jurisdiction. 

#### Phase II: Signalling

1. **Prediction market creator (integration with our project wizard)**

The parameters for prediction markets must be based on the structure of the social projects hosted on the Alice website. We want to automate the process of deployment and configuration of gnosis contracts. The solution is going to be implemented as a process that will monitor the state of Alice donation contracts and once it detects that the contracts are fully approved and operational it will deploy the matching prediction market contracts and set up all of the necessary references. It will handle the gas payments, transaction monitoring and error handling.

The solution will be fully open-sourced and will hopefully provide a reference implementation for other projects to automate integration with the Gnosis protocol.

2. **Market monitoring dashboard**

Fetching all of the data through a web3 protocol could be a slow and frustrating experience for users who are used to fast loading dashboards. If we want to integrate multiple prediction market monitoring on the investors dashboard we should implement a solution that will speed up the initial loading process. Moreover, the Alice platform attracts mainstream donor for whom getting the web3 browser only to check the status of a prediction market may not justify the effort of installing proper tools. 

Therefore, we want to implement the proxy and caching layer to fetch data and store it into an intermediary database for fast access. We already have extensive expertise in this, gained through our experience of building Etheroscope, an open-source smart contract explorer. We hope that these solution may boost adoption of prediction markets especially among less tech savvy users who’d like to monitor the market before making the effort of installing necessary tools and actively interacting with the contracts.

3. **Market tracking notification**

Prediction market mechanism offered by gnosis could be a powerful tool to get instant warning if a social project is facing challenges that may affect its success rate. The instant reaction and involvement from the side of social impact investors may often help to put the project back on track and reduce the risk of not achieving the promised goals.

Therefore, we are going to implement an instant notification module that will directly inform engaged parties when there is sudden change in the prediction market. The solution will be built as a monitoring daemon which will listen to the smart contract events and determine when a market alert should be triggered. The monitoring process will be connected to a messaging service that will automatically notify the previously specified recipients. 

4. **Special-purpose beneficiary wallets**

We are going to design and implement a special purpose wallet that will be funded with air-dropped tokens for beneficiaries. The wallet will restrict the token usage only to the specific market that the beneficiaries participate in. It will also control the investment flow reducing the risk of sudden spending and speculation.

5. **Project feedback interface for beneficiaries**

We cannot assume that beneficiaries are either tech-savvy or blockchain experts. Therefore, the usability of the interface for reporting project progress are key requirements for this module. 

We are going to integrate with browser-based ephemeral wallet such as the [burner-wallet](https://github.com/austintgriffith/burner-wallet) to remove the need of installing extra tools. We also plan to use gas-less transactions support by leveraging the technology offered by [gas-network](https://medium.com/tabookey/1-800-ethereum-gas-stations-network-for-toll-free-transactions-4bbfc03a0a56) or other similar [meta-transaction](https://meta-tx.github.io/) solutions. The final design of the interface will be based on our experience in implementing highly accessible blockchain solutions like our [donation app](https://donationsapp.alice.si/). We believe that the implementation of prediction markets with the focus on usability and accessibility of the final interface could boost the adoption of similar projects based on the gnosis infrastructure. 

### Team description

**Raphaël Mazet**

Before co-founding Alice, he was co-founder of CliqStart, a digital activism startup focused on charity advocacy campaigns. Before becoming a social tech entrepreneur, he spent ten years managing a team responsible for corporate communications in Europe and Latin America. Raphaël is Franco-British and trained as a political scientist at the London School of Economics and Sciences-Po Paris. He’s actively engaged in the blockchain space for over 3 year as an expert and conference speaker. He’ll work as a project manager. 


**Jakub Wojciechowski**

Jakub is a software engineer specialised in blockchain technology and financial services. He has a Master’s degree in computer science from the University of Warsaw, where he also obtained an undergraduate degree in economic psychology. Before co-founding Alice, Jakub was the founder of Silvertown, a proptech company powered by the blockchain and using IoT to automate the management of large social housing estates. Prior to this, he worked for several years at Efinity, a Polish insuretech startup, and as a flex and java consultant for financial sector clients at Infovide-Matrix. He’s contributing to various open-source projects like: OpenZeppelin, Etheroscope, SensorTrx  and speaker of a few Ethereum tech-conferences including devCon, ethCC, Ethereum London Meetup. He also runs a Warsaw Smart Contracts Code Club. He’ll work as a blockchain developer. 


**Areti Kampyli**

Areti has a background in advertising, communication and design. She started her career in advertising at Ogilvy & Mather, where she managed clients including Delta Airlines and BT. She launched her first tech startup in 2009 and prior to Alice, Areti was CEO of CliqStart. She is a London School of Economics graduate, where she did her MSc in media and communications. She will be responsible for the UX design, implementation and user testing. 

**Alex Suvorau**

Alex is a software engineer. He studied computer science program at the University of Warsaw. Before joining Alice Alex worked as a software engineer at Polish software agency Atinea. He’s a winner of national mathematical competition of Belarus. He’s been passionate about the blockchain space for two years attending a few hackathons and working on his own projects. He’ll work as a full-stack developer. 

**Dhen Padilla**

Dhen is a software engineer, with a background in UI/UX and machine learning. He has worked on projects with Nuffield Health and NHS Royal College of Surgeons, designing and producing interoperable Web & iOS Applications. Dhen is presently pursuing his MEng at University College London, specialising in decentralised network anonymisation and deep learning. He’ll be responsible for front-end development. 


### Timeline, Milestones and Deliverables

**Phase I: Social impact investing protocol**

**1. Implementing impact investments as smart-contracts powered by conditional tokens**
 
**Deliverables:**

  * Use conditional tokens as a base building block for tokenized impact investments
  * Implement the investment creation factory
  * Implement the investment and interest repayment flow
  * Integrate the conditional token splitting/merging mechanism as a way to increase liquidity

**Time and price estimate** - 1 month, $6,250

**2. Social impact investment management platform**
 
**Deliverables:**

  * Implement UI for creating/funding social impact investments 
  * Implement UI for splitting/merging bonds
  * Implement the integration with Alice’s donation and validation (impact oracles) modules

**Time and Price Estimate** - 2 months, $12,500
 
**3. Social impact investment controllers**
 
**Deliverables:**

  * Specify the generic regulatory requirements
  * Implement smart-contract powered controllers mediating interactions with bond contracts to assure following the regulatory requirements 
  
**Time and Price Estimate** - 1 month, $6,250
  
**Phase II: Signalling**

**1. Integrating Gnosis markets as a signaling tool for the Alice platform**
 
**Deliverables:**

  * Integrate market deployment into the project creation wizard
  * Integrate market monitoring into the Impact tracking dashboard
  * Integrate market events into the donor feedback mechanism
  
**Time and price estimate** - 2 months, $12,500
 
**2. Building an app for beneficiaries to provide feedback about project status**
 
**Deliverables:**

  * Implement a special purpose wallet in the form of a pre-funded smart-contract proxying the interaction with the prediction markets
  * Build a convenient interface for beneficiaries to report progress of the social project
  
**Time and Price Estimate** - 2 months, $12,500


