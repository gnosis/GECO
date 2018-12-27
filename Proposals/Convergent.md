# GECO Proposal

## Project Overview

### Project name
[Convergent](https://convergent.cx)

### Team members
Logan Saether
Achill Rudolph

### What project are you building
Convergent is an open source, extensible cryptoeconomic social network that enables creators to launch a token and build an ecosystem around it. We want to extend this project by adding modules for personal prediction markets that take the form of polls and a futarchy app which allows followers to make governance decisions for individuals. Users will not only be able to invest in personal tokens and benefit from their long term growth, but also to influence and bet on concrete actions, decisions and outcomes of tokenized individuals.

### Why did you decide to build it
Market mechanisms that allow people to invest in and take part in determining the future of organizations and corporations have existed for many years as shareholder agreements. As we imagine the social networks of Web3, we believe the key innovation is the underlying vein of value constantly being transacted. To enable individuals and creators to tap into this latent network of social value of their work, time, attention, or future we decided to build our project. 
 
We want to make these features accessible to smaller organizations down to the singular individual. Personal prediction markets, in the form of polls, could become one of the most exciting and engaging user experiences of our product. It forms the base for the more advanced application of an entire futarchy extension to our base platform that we believe is beneficial to the entire ecosystem.

### How long will it take
5 months

### How much funding are you requesting
€8,000 / month --- €40,000 total for 5 months
### How did you hear about the GECO
Word of mouth, then Twitter and Medium post by Mareen Gläske.

## Your Proposal

### Project description
_Outline a detailed description of your project, why you chose to build this project, the overall goal and future outlook of your project and why we should fund you._

Convergent is pioneering the realm of personal token economies: We allow individuals to create and interact through cryptoeconomic mechanisms around their personal brand. 

To illustrate the basic mechanism consider the following example: A young author who is writing her first book launches a personal token and promises 1 signed copy of the book to anyone who pays her 1 of her personal token. If the author is trusted to actually honor her commitment, the token will come to represent the market value of 1 signed copy of the book, even when the book does not exist, yet. People can buy and sell that token from a bonding curve contract (i.e. without an ICO and without having to go through an exchange). If someone discovers early that the book will become a success, they can benefit from this by investing in the author’s personal token and selling when demand has grown. We expect this to become useful in particular for people who have to build a personal brand and find ways for their audiences to engage with it: artists, content creators and the ever growing independent work-force at large. But the mechanism can be used to tokenize many other kinds of goods and services, not just future artistic creations, but also attention, influence, governance, expertise, or simply time.

The project has three distinct touchpoints with Gnosis which we would like to expand with the help of GECO funding. First, we are conducting research in novel market mechanisms and cryptoeconomics. Second, we want to integrate Gnosis prediction markets as the next feature in our product. And third, we are prototyping and testing futarchy for personal economies. In the following, each of these three touch points is described in detail:

#### 1. We are researching personal prediction markets.

Our product allows individuals to tokenize their work, time, or attention and raise funds from supporters who believe that these aspects of the individual are currently undervalued. Although it does not follow the traditional setup of a prediction market, our core protocol is in some sense a continuous personal prediction market. However, the bonding curve allows for novel business models, thereby giving this prediction market an additional feature: It not only incentivizes participants (henceforth referred to as contributors) to predict and discover successful individuals, but also helps those individuals (henceforth referred to as creators) to fund investments in their personal growth. We are researching the technology and cryptoeconomic primitives that can make such alternative personal prediction markets sustainable and useful for all parties involved.

#### 2. We are integrating a standard prediction market, using the Gnosis platform.

The core feature of our product allows creators to generate their own currency and back it with their offered services. Contributors may then invest in the personal brand and personal value streams of the creator and benefit from that creator’s long-term growth. To create a more engaging day-to-day user experience, we want to extend the platform with more direct opportunities for cryptoeconomic interaction. Predictions are one of the most intuitive and natural ways of interacting with our social environment: When we think about the people and organizations we care about, we wonder what choices they will make and what will happen to them. Therefore, with the help of GECO, we want to include prediction markets, in the form of polls, as the first cryptoeconomic extension of our platform.

#### 3. We are experimenting with futarchy.

Another interesting interaction of prediction markets and personal economies is to be found in futarchy. We believe that prediction markets can be used to elicit good decisions - not only for governments and firms, but also for individuals and small organizations. We want to experiment with this idea and build a basic prototype to test it.

In conclusion, our work is highly relevant to Gnosis’ vision of redistributing the future. However, we are at a very early stage with this project and do not plan a token launch for fundraising in the near future. Even within the blockchain ecosystem our field is very experimental and research-heavy. We are also radically transparent, open source and community driven. Altogether, this makes funding through traditional sources hard. Therefore we rely on securing a grant for this work. We would appreciate any support at this critical moment in the project lifecycle. We would work our asses off to leverage it most efficiently and make our vision of redistributing personal futures come true.

### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._

The [current prototype of the Convergent platform](https://proto.convergent.cx) already allows users to launch their own token economy and endow their token with value by linking it to offered services. We are currently using React JS for the frontend webapp, Solidity for smart contracts and Drizzle to connect the two. We are deploying and testing contracts with Truffle. For consistency, the features described in this proposal will be built using the same technology stack.

The project encompasses the technical implementation of point 2 and 3 from the project description above. Both will be built by integrating the existing Convergent platform with Gnosis’ smart contracts and interfaces.

#### A. Standard Prediction Markets Integration

The integration of standard prediction markets into the personal economy platform will be the main feature to be built as part of this project. This extension will allow users to open prediction markets about their personal future with an integrated interface on their Convergent profile page. It will look reminiscent of social polls on web 2.0 platforms. However, a prediction market will be a far more engaging experience for web3 users because it entails real skin in the game, thereby making the game more exciting.

In all likelihood, most of these personal prediction markets will be small in size and therefore not highly profitable or significant in financial terms. Nevertheless, they can be immensely valuable and entertaining for many groups of supporters as a new direct way of interacting with the creators and organizations they care about. The creator on the other hand would gain valuable insights into the sentiment and opinions of her audience. The prediction market would give her an additional instrument to harness the wisdom of her crowd and create engagement around her personal brand. The main challenge for the technical implementation, will be to create a UX that conveys this spirit and adapts the standard setup to the personal economy context. The main outcome of this project will be a complete software module that will make it fun and rewarding to set up, interact with and analyse low-stake personal prediction markets.

Furthermore, the combination of prediction markets and personal bonding curve tokens results in interesting new cryptoeconomics. For example, we are planning to allow the use of personal tokens as the reserve currency for the personal prediction market. This improves incentive alignment and provides more value to the personal token as a focal point for the personal economy of the creator.

#### B. Personal Futarchy Prototype

As the second deliverable of this project scope, we will build a basic prototype to explore a potential extension of the standard prediction market setup. Rather than just opening a market for predicting a future outcome, users might also want to elicit the crowd’s wisdom to actually help them make decisions and shape their future. We will create a prototype that integrates this extension into the Convergent platform, conduct comprehensive user tests and document the results.

We are already seeing existing use cases, where the creator of a personal token economy allows token holders to influence her decisions. Most people would not give personal life decisions away to an open market (though there are some isolated instances of this). However, when the token represents the professional identity of an individual or a small organization, governance and decision rights can easily be conceived as a core part of the token economy. For example, the existing Jonas Lund Token gives its holder “agency over future decisions concerning Jonas Lund's artistic practice”.

Futarchy provides a promising variation of this model. Rather than allowing token holders to directly vote on the decision of the creator, they could enter a conditional prediction market and let the outcome of that prediction market determine the creator’s decision. This is similar in spirit to the idea of Futarchy Curated Registries, as pioneered by Gnosis in cooperation with Chris Whinfrey and Level-K. Personal token economies provide the perfect testing ground for such models because they provide many opportunities for low-stake, yet exciting and fun decisions.

### Team description
_Who are your team members, what is your background and what you built before._

[Logan](https://github.com/lsaether) is a professional smart contracts engineer with a humanistic background. He started coding at the age of 12 and went on to study complex systems and English literature. Before initiating Convergent, he rebooted and maintained the Ethereum Alarm Clock (a protocol for scheduling Ethereum transactions) as a developer at ChronoLogic and conducted research into a similar protocol for the scheduling of meta-transactions. He offers code reviews and security audits on a case-by-case basis through his [audit firm](https://trustless.design).

[Achill](https://github.com/acrdlph) is a rigorous economist, self-taught full-stack developer and passionate entrepreneur. He studied philosophy and economics at Bayreuth, Harvard and Yale. Over various career steps he gained extensive experience in quantitative economic research, business strategy and product management. Before initiating Convergent, he was the co-founder and CEO of Way Network and built its [beta prototype](https://cryptogeeks.berlin), a decentrally curated local chat app. He is also an Ethereum community organizer regularly hosting the Curation Markets meetup in Berlin.

We met in September 2018 and discovered our shared interest in continuous bonding curves and personal token models. After some prototyping and hackathon implementations, we started working full-time on the idea in early November. Ever since, we are working together around the clock. We are both fully and indefinitely committed to this project.

### Timeline, Milestones and Deliverables
We divide the work up into two large chunks with smaller deliverables every two weeks.

#### Phase I (3 months) - Prediction Markets "Polls" and Integration
During this phase we will build the poll front-end to the prediction market contracts and work on integration of it into our platform.

| Deliverables   | Time         | Price        |
| :------------- | :----------: | -----------: |
| Preliminary research, wireframes and specification of integration | weeks 1-2    | €4,000    |
| First standalone prototype of polls tool | weeks 3-4    | €4,000    |
| Optimizations and UX testing   | weeks 5-6    | €4,000    |
| Complete standalone version of polls tool | weeks 7-8    | €4,000    |
| Integration into personal economies platform (contributor perspective) | weeks 9-10   | €4,000    |
| Integration into personal economies platform (creator/dashboard perspective) | weeks 11-12  | €4,000    |

#### Phase II (2 months) - Futarchy Application
This phase will build on the work we accomplished by building the prediction markets poll app and research and build a working futarchy application on top.

| Deliverables   | Time         | Price        |
| :------------- | :----------: | -----------: |
| Futarchy research report, detailed specification and wireframes of futarchy app | weeks 13-14  | €4,000    |
| Create interface from contributor (voter) perspective | weeks 15-16  | €4,000    |
| Create Dashboard interface for creator perspective, UX feedback on front-end | weeks 17-18  | €4,000    |
| Complete futarchy application on personal economies platform | weeks 19-20  | €4,000    |



### Others
We have applied to the Ethereum Community Fund, the Samsung NEXT Stack Zero Grant, Consensys and several other investors but have not received any responses so far.

Here you can find our current live prototype on the Rinkeby testnet: https://proto.convergent.cx All our work is done in plain sight and we constantly share updates through our public channels: https://convergent.cx/, https://github.com/convergentcx, https://twitter.com/ConvergentCx, https://discordapp.com/invite/JUPx5Xg, https://medium.com/convergentcx. 

We know this is new but innovation requires courage and boldness. Thank you for your consideration.
