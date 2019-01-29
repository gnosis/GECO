## Project Overview
<p align="center">
  <img src="https://github.com/flyingcarpet-network/GECO/blob/master/Proposals/assets/Flyingcarpet/FLCA_logo.jpg" />
</p>

### Project name
Flyingcarpet Network

### Team members
Julien Bouteloup - https://www.linkedin.com/in/jbouteloup/

Leopold Joy - https://www.linkedin.com/in/leopoldjoy/

Victor Faramond - https://www.linkedin.com/in/victorfaramond/

Mike Onorato - https://www.linkedin.com/in/mikeonorato

Satya Doraisamy - https://www.linkedin.com/in/satya-doraisamy-a51962104/
### What project are you building
At Flyingcarpet, we are building a decentralised geospatial layer for Earth Observation. The Flyingcarpet Network incentivises data scientists to build an open library of geospatial analytics-extraction models. Analytics are made continually available to paying organisations via our Analytics API, which will also function as an oracle that can be integrated directly into smart contracts. Models are tokenised so that anyone can invest in them and share in their future revenue.

As a component of the Flyingcarpet Network, we are creating two Flyingcarpet prediction markets on top of the Gnosis PM v2.0 smart contracts. The first, our Flyingcarpet Predictions Dashboard, will enable anybody in the world to make  predictions from Flyingcarpet model insights. The second, our Model Viability Prediction Market, will be a conditional prediction market, enabling Flyingcarpet users to bet on the future profitability/demand for models that haven’t been created yet.


#### Flyingcarpet Network Workflow

1. Model Viability Prediction Market (Gnosis Integration): A Gnosis PM v2.0 conditional prediction market crowdsources sentiment from Flyingcarpet Network participants to determine the prospects of future models (how the Flyingcarpet community predicts the future profitability/demand of, for example, a model that analyses Amazonian deforestation vs a model that analyses Arctic ice melt). See Model Viability Prediction Market section below.
2. Model Sourcing: Data scientists produce optimal models for the paying organisation’s request. Effective models are stored decentrally with all computation taking place off-chain.

3. Models Dashboard & Predictions Dashboard (Gnosis Integration): The Flyingcarpet Predictions Dashboard enables participants to make predictions on physical-world events with models acting as arbiters of truth. Analytics from Flyingcarpet models are made continually available to paying organisations via our Analytics API and smart contract oracles.
4. Model Investments and Financial Instruments: Models are tokenised and converted into investible entities that can function as financial instruments (see Additional Decentralized Financial Instruments section below) so that anyone, anywhere can capture the value of Earth observation.

### Why did you decide to build it
Julien picked this idea because he had previously worked on building AI-powered IoT swarms. The increasing number of Earth observation satellites, combined with recent advances in both machine learning and blockchain led to a greater vision: using blockchain-based incentives to build a decentralised library of machine learning Earth observation models.

Earth observation satellite imagery has such broad applications across all organisations and industries that it will be a key driver of economic growth in the next decade and beyond. However, since such analytics are currently provided by centralised and pricey firms, only organisations with considerable financial resources can access geospatial analytics. As a result, many organisations that would benefit the most from these analytics, such as SMEs, non-profits, NGOs and humanitarian efforts, are priced out.

In a world where economic inequality is increasing and power is becoming increasingly centralised, we at Flyingcarpet are determined to ensure that the value of Earth observation is open to everyone. We envisage that Flyingcarpet will massively increase organisational access to Earth observation analytics—and predictions built on these insights—while also distributing value to data scientists in a fairer way.


### How long will it take
Eight months, split between two milestones (four months each).

### How much funding are you requesting  
**$80k total funding. Breakdown:**
1. **$40k: Feb - May 2019** — Concurrent development of the Flyingcarpet Predictions Dashboard and the Flyingcarpet Model Viability PM Dashboard. This front-end development will entail creation of both web3-enabled Dapps.
2. **$40k: June - Sept 2019** — Full integration of Predictions Dashboard with all existing and future Flyingcarpet models (e.g. coffee, ice melt, deforestation, catastrophes etc.) so that users can start making predictions on Gnosis PM with Flyingcarpet oracles as more come online. Also, back-end development of Model Viability PM Dashboard, including integration with both Gnosis and Flyingcarpet smart contracts, followed by a marketing push to drive our community of data scientists and paying organizations to participate in this Gnosis PM.

### How did you hear about the GECO
Website

## Your Proposal
### Project description
**The Flyingcarpet Predictions Dashboard**

A Flyingcarpet Predictions Dashboard will open up more uses for our decentralised Earth observation models. The Flyingcarpet Predictions Dashboard will enable anyone to bet on events relating to the physical world insofar as a Flyingcarpet model exists for a particular prediction. Flyingcarpet models will serve as oracles and provide a single source of truth for these predictions, thereby allowing bets relating to the physical world to be made in a trust-minimised manner and without a rent-seeker acting as an arbiter of truth.

We envisage that the Flyingcarpet Predictions Dashboard will be popular with corporate entities that already plan to use Flyingcarpet for their operations as a way to hedge against unfavourable events. For example, one of our clients is a multinational coffee trader that is using a Flyingcarpet model to estimate crop yields in Brazil; the Flyingcarpet Predictions Dashboard will enable this specific client to hedge against a poor yield using analytics extracted by the same model. We believe that corporates will be some of the biggest users of secure prediction markets, since bets can often amount to disintermediated insurance; the Flyingcarpet Predictions Dashboard will aim to accelerate this future.

We anticipate that some models, such as those relating to climate change and the environment, will attract larger volumes of prediction market users. We are building a model in partnership with Ice Alive, for which we recently received a grant from Microsoft and National Geographic, that monitors glacial melt in the Arctic and a model for Reforestum that monitors biomass in order to measure CO2 reductions. In the case of the former, we anticipate that everyone from NGOs to researchers engaged in tackling Arctic ice melt will have an incentive to bet on the precise rate of glacial melt. Regarding the latter, individuals and organisations that purchase carbon offsets (an immense market) would have an incentive to bet that CO2 reductions are increasing.

For both of the above climate-related use cases, we believe that corporations and high net worth individuals may use prediction markets to indicate in a transparent and cryptographically secure way to the public that they have serious “skin in the game” vis-à-vis the causes that they profess to champion.
<p align="center">
  <img src="https://github.com/flyingcarpet-network/GECO/blob/master/Proposals/assets/Flyingcarpet/gnosis_prediction.png" />
</p>

**The Model Viability Prediction Market Dashboard**
The Flyingcarpet Network will source optimal models for particular use cases by incentivising data scientists with bounties. Optimal models are then stored decentrally and made available to analytics-hungry organisations.

Flyingcarpet will integrate the Gnosis PM v2.0 smart contracts with our Model Viability PM Dashboard front-end in order to enable participants to make bets about the future demand for, and financial profitability of, potential models (e.g. predictions like “if a model for soybeans in the United States gets created, will it generate $100k of revenue in the first 6 months?”). All Flyingcarpet Network participants, including data scientists, satellite imagery providers and paying organisations, have a vested interest in what model use cases get created. Our initial models are being built based on direct relationships with clients, however since the Flyingcarpet Network will be fully decentralised, it needs an ongoing mechanism to crowdsource sentiment from network participants in a trustless manner; therefore, this is an ideal use case for a prediction market.

Given the volume of Flyingcarpet participants that will have an incentive to participate in the Model Viability Prediction Market, we anticipate that this integration will bring substantial users to Gnosis’ platform. Once Flyingcarpet attracts large numbers of data scientists, network effects will kick in and we expect large businesses to participate in the Model Viability Prediction Market in order to leverage Flyingcarpet data scientists to suit their needs, which will further drive activity on Gnosis’ platform.

### Features
Below we will expand on the technical features of our two Gnosis prediction markets and outline some additional financial instruments we intend to develop on top of Gnosis.

**The Flyingcarpet Predictions Dashboard**
The Predictions Dashboard functions as a front-end interface where users can interact with Gnosis predictions that use analytics from Flyingcarpet models. This web3-enabled dashboard will be integrated with both the Gnosis PM and Flyingcarpet smart contracts.
While the Flyingcarpet contracts will provide model information (e.g. what model oracles are available), the Gnosis PM contracts will function as the interface for all predictions based on Flyingcarpet insights, allowing prediction bets to be created and sending back event outcome information.

The Flyingcarpet smart contracts only contain hashes (e.g. IPFS) corresponding to models and their extracted analytics, as models are both stored and executed off-chain. The Flyingcarpet smart contract will provide Gnosis PM smart contracts access to extracted model analytics (e.g. to determine event outcomes).

<p align="center">
  <img src="https://github.com/flyingcarpet-network/GECO/blob/master/Proposals/assets/Flyingcarpet/FC_Gnosis_workflow.png" />
</p>

**Model Viability Prediction Market Dashboard**
Predictions regarding the demand / profitability of future models will be used to gauge the interest of the Flyingcarpet community with regard to model creation options (e.g. a corn yield model vs a large cargo ship counting model). Since this application requires conditional market support (e.g. predictions of the format: “if x model is built and x model is arbitrarily profitable/in demand”), it is an ideal use case for Gnosis’ new v2.0 PM contracts which enable conditionals.
<p align="center">
  <img src="https://github.com/flyingcarpet-network/GECO/blob/master/Proposals/assets/Flyingcarpet/Model_Viability_Prediction_Market_Dashboard.png" />
</p>

**Additional Decentralized Financial Instruments**
In addition to the aforementioned Flyingcarpet prediction markets, we plan to construct a number of other financial instruments on top of Gnosis, including:
1. Partial model ownership tokens (see Whitepaper) as collateral against loans and predictions on Flyingcarpet’s (Gnosis) Predictions Dashboard.
2. Trading of partial model ownership assets on DutchX exchange contracts.
3. Integration of Gnosis Safe for storing partial model ownership tokens and interacting with Flyingcarpet PMs and our future DutchX exchange integration.

### Team description
**Julien Bouteloup, CEO**

Julien holds a Master’s degree in electrical engineering from the USA and a Master’s degree in electrical engineering from France, where he specialised in artificial intelligence, decentralised systems and security back in 2009. He has built multiple tech businesses ranging from energy trading, high frequency trading, decentralised identity to autonomous transportation systems and won multiple competitions worldwide. He was first introduced into Bitcoin in 2010 and then Ethereum in 2015. He is a full-stack engineer and developer, a regular speaker at Ethereum and Blockchain conferences, including Devcon. He teaches blockchain in London (https://www.theblockchainconnector.com/meet-the-team), advises OECD (Organisation for Economic Co-operation and Development), ADB (Asian Development Bank) and BBA (British Blockchain Association).


**Leopold Joy, Lead Developer**

Leopold is a full-stack software developer. He taught himself to program at the age of 13 and founded and built his first startup at the age of 15. As an undergraduate he studied Computer Science at Bard College and the Rensselaer Polytechnic Institute (RPI), both in New York. Leo has extensive experience in open-source software development, Ethereum and blockchain, and co-founded a number of early stage startups, including an early large-scale Monero mining operation and campus messaging app. He is an active member of the open-source blockchain community and excited to radically disrupt the geospatial analytics space with Flyingcarpet.


**Victor Faramond, Developer**

Victor is a full-stack developer with an MSc in maths and computer science. He founded MoonPay, a credit card facility for purchasing crypto and is the Head of Engineering at Hodl.vc. Previously, he completed an 11-month software engineering internship at Apple.

**Mike Onorato, Developer**

Mike received his B.S.E. from Princeton University with a senior thesis in machine learning and a certificate in robotics and intelligent systems. He has extensive startup software engineering experience and, most recently, worked as a Senior Software Engineer at DroneBase, building next-generation software for drones.

**Satya Doraisamy, Legal Lead**

Satya has experience in investment banking and venture capital, and has also founded Nebula Learning, an education startup. At Flyingcarpet, he handles legal documentation, assists with business development, and co-authored the white paper.

### Timeline, Milestones and Deliverables
**Phase I: Front-End Development Prediction Market Dashboards**

**Deliverables:**

1. **Complete development of Flyingcarpet Predictions Dashboard:** the Predictions Dashboard, a web3-enabled dApp, will be a fully featured UI enabling users to interact with predictions based on Flyingcarpets model oracles. Users will be able to make predictions directly from the interface, as well as view charts/graphs of relevant historical analytics extracted in the past.


2. **Complete development of Flyingcarpet Model Viability Prediction Market Dashboard:** Another web3-enabled dApp, the Model Viability Prediction Market will provide Flyingcarpet community members with a market to bet on the future profitability and demand for new models. The dashboard will provide a UI to compare these conditional predictions and view details about the function of, and market for, each potential future model. Users will be able to view their existing bets and submit new ones via an intuitive UI.

**Time and Price Estimate:**
$40,000 and completed by end of May 2019. This money will be used to take the pressure off our development teams who are currently self-funding the project.

**Phase II: Back-End Development of Prediction Markets + Scaling and Launch**

**Deliverables:**

1. **Flyingcarpet Predictions Dashboard Back-End:** We will integrate the Predictions Dashboard with both the Gnosis PM v2.0 smart contracts and the Flyingcarpet model management smart contracts—these Flyingcarpet contracts will also talk directly to the Gnosis PM contracts (see earlier diagram).

2. **Integration of Models with Predictions Dashboard:** We will integrate existing Flyingcarpet models with the Predictions Dashboard (e.g. the coffee yield model for our client Sucafina, a multinational commodity trader). The dashboard will then be setup to provide predictions for all future models as they come online—for example: our glacial melt model with Ice Alive (via a partnership with National Geographic & Microsoft), our various insurance catastrophe models with Nephila and AXA and our deforestation model for Reforestum, a platform for purchasing carbon-offsets.

3. **Flyingcarpet Model Viability Prediction Market Back-End:** We will integrate the Model Viability Prediction Market Dashboard with the Gnosis PM v2.0 smart contracts to provide the backbone of the Flyingcarpet community evaluation platform for future models.

4. **Drive Adoption of Model Viability Prediction Market by Flyingcarpet Community:** We will continue to develop a strong community and begin to query the sentiment of the community about future model possibilities. This will drive Flyingcarpet community members to Gnosis (via our Model Viability Prediction Market). Because our team is currently very developer-heavy, we will need to hire the necessary talent to grow a strong marketing team to ensure continued community growth and engagement.

**Time and Price Estimate:**
$40,000 and completed by end of September 2019. We will use this money to fund development of the back-end of the PM dashboards, integration of Flyingcarpet models and to incentivise marketing people to join our team.
