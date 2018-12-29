# Tasit SDK

## Project Overview

### Project name

> [Tasit SDK](https://github.com/tasitlabs/tasitsdk)

### Team members

> Paul Cowgill, Marcelo Morgado

### What project are you building

> The Tasit SDK is a JavaScript SDK for making standalone native mobile Ethereum dapps using React Native.

> Here's a video of Paul Cowgill pitching Tasit Labs (the company doing most of the initial work on the Tasit SDK): https://youtu.be/PPbwf1-4Jpk

> [tasit.io](https://tasit.io)

### Why did you decide to build it

> I often feel frustrated that I can't use Ethereum dapps on my mobile phone the way I would with any "web 2" app. For instance, sometimes I want to add someone to the Aragon DAO for my meetup group on my phone when I meet them at a meetup, but instead I have to set a reminder to do it when I'm back at my computer at home. If I'm noticing this inconvenience as someone who's technical, the average potential user must feel that pain even more. The Ethereum community loses mainstream people from the onboarding funnel because of this.

> The 3 main source of friction are:
> A) Using a dapp within a browser dapp is an unacceptable UX. Almost all legitimate experiences on mobile today happen in standalone native apps.
> B) As someone who already has ETH and tokens, needing to transfer some of these funds permanently from my preferred mobile wallet to another account in order to use a dapp is an unacceptable UX.
> C) Needing ETH or tokens in the first place to try a dapp is too much onboarding friction.

> These problems can be solved with a JavaScript SDK for writing mobile apps for Ethereum dapps in React Native with a few advanced onboarding features built in. This helps developers build new mobile dapps more quickly without reinventing the wheel for basic features.

### How long will it take

> We will need 3 months to ship version 1.0.0 of the project.

### How much funding are you requesting

> \$34000

### How did you hear about the GECO

> Talking with engineers from the Gnosis team at Devcon4

## Your Proposal

### Project description

##### A detailed description of your project

<!-- TODO: Add me -->

_{ Coming soon }_

##### Why you chose to build this project

See the "Why did you decide to build it" section above.

Also:
https://github.com/tasitlabs/TasitSDK/blob/develop/README.md#why

##### The overall goal and future outlook of your project

<!-- TODO: Add me -->

_{ Coming soon }_

##### Why we should fund you.

<!-- TODO: Add more -->

_{ More coming soon }_

React Native is an especially great fit for mobile dapps since React is such a commonly used technology for web-based dapps - this allows for more code reuse.

### Features

_There are more specifics on the features in the deliverables sections below._

##### Tools and frameworks

ethers.js, React Native, Expo, Jest, Truffle, Babel, Infura, Lerna, smart-contract-based wallets (Gnosis Safe in particular), meta-transactions, ERC721, ERC165, Fastlane, CircleCI

##### Architecture, mockups, etc.

- [Architecture](https://www.dropbox.com/s/gw88c5ua4ssthvg/TasitProjectStructure.png?dl=0)

- A README with [more details on the Tasit SDK](https://github.com/tasitlabs/TasitSDK/blob/develop/README.md)

- A README with [more details on the Tasit apps](https://github.com/tasitlabs/tasit/blob/develop/README.md) - all the mainstream-user-facing apps for popular web-based dapps (like Decentraland, Aragon, etc.) that will be built using the Tasit SDK

- [Slides about the Tasit SDK](https://bit.ly/2018-12-04-chicago-ethereum-meetup)

- [Video with example app onboarding flow](https://youtu.be/iJQtDPQrRsE) (interactive wireframes)

- [Demo app using the Tasit SDK](https://github.com/tasitlabs/tasit/tree/develop/demo)

### Team description

##### Paul Cowgill

[LinkedIn](https://www.linkedin.com/in/pcowgill/) // [Twitter](https://twitter.com/paulcowgill) // [GitHub](https://twitter.com/paulcowgill)

Paul recently worked on a smart contract audit for OpenZeppelin 2.0 with the team at Level K (plus a few other high-profile audits). For the past year and a half he has been working as a freelance software engineer specializing in Solidity, IPFS, Truffle, React, and React Native.

He has a lot of experience working on native mobile apps, most recently including the Heatworks mobile app. Before that he was the first hire and CTO at the YC-backed IoT startup Edyn - he wrote the initial code for much of the tech stack (Node.js, AWS, mobile, etc.), and as CTO he led the growth of the software and data science teams to 12 people. The Edyn team shipped 10,000 units of their IoT products and continuously iterated on a production mobile app to use with them.

_Education_

He did his undergrad at Princeton in Electrical Engineering, and his masters at Harvard in Systems Biology.

##### Marcelo Morgado

[LinkedIn](https://www.linkedin.com/in/marcelo-morgado/) // [Medium](https://medium.com/@marcelomorgado) // [GitHub](https://github.com/marcelomorgado)

Marcelo is a full-stack developer with >5 years of experience and a sysadmin with >10 years of experience. He has participated in and lead several software development projects. Cryptocurrencies/decentralization and open-source enthusiast.

Marcelo has personally faced the problem that we're trying to solve. He participated in a Status Hackathon in September 2018. The web app he built is functional but the React Native mobile project still only is a prototype, because he didn't have enough time to build an Ethereum wallet from scratch and then build a dapp during the hackathon. He has been following crypto technologies for 4 years now, and he thinks that one of the greatest barrier to the mass adoption of crypto and dapps is the friction with handling private keys, identity, and gas.

_Education_

**University of Nicosia**
DFIN-511 Digital Currencies
2018 - 2018

**PUC-Rio** (#1 Brazillian private university - 2018)
Bachelor’s degree, Information
Systems
2006 - 2013

### Timeline, Milestones and Deliverables

**Phase I - v0.1.0**

**Deliverables**

- Ephemeral account and private key generation

- Higher-level abstraction for reading and writing data and reacting to events

- Advanced support for ERC721

- Onboarding using the Gnosis Safe for users with funds in there already

- Proof-of-concept app for Decentraland on TestFlight for iOS on a testnet

**Time and Price Estimate**

1 month, \$16500 total

- \$2000 design contract work

- $13500 1 month of $6,750/month pay for 2 software engineers

- \$500 SAAS costs, like an Apple Developer Program account to have a test implementation of an app using the SDK, etc.

- \$500 legal costs with Stripe Atlas

**Phase II - v1.0.0**

**Deliverables**

- Advanced support for one of these: (A) DAOs, (B) TCRs, or (C) two-sided marketplaces.

- "tasit init" scaffolds out a mobile dapp

- Onboarding using the Gnosis Safe for users new to Ethereum

- Configurable JSON-RPC client

- Proof-of-concept app for Decentraland on TestFlight for iOS and Google Play beta track on mainnet

**Time and Price Estimate**

2 additional months, \$17500

- \$2000 design contract work

- $13500 1 month of $6,750/month pay for 2 software engineers (salary for the 3rd month to be secured from elsewhere)

- \$2000 travel to conferences to speak about the project and attract other developers to use and/or contribute to the SDK.

**Phase III**
We have plans for phase III and beyond, but I'm intentionally keeping the scope of this initial grant request smaller.

### Other

- [Website](https://tasit.io/)

- [Twitter](https://twitter.com/tasitlabs)

- [Project Kanban board](https://github.com/orgs/tasitlabs/projects/1)

- [Telegram](https://t.me/tasitlabs)

- [Email](mailto:founders@tasit.io)

- [Feature requests](https://tasit.canny.io/feature-requests)
