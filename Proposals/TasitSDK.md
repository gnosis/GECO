# Tasit SDK

## Project Overview

### Project name

> [Tasit SDK](https://github.com/tasitlabs/tasitsdk)

### Team members

> Paul Cowgill, Marcelo Morgado

### What project are you building

> The Tasit SDK is a JavaScript SDK for making standalone native mobile Ethereum dapps using React Native. It integrates seamlessly with the Gnosis Safe so that mobile dapps can use funds stored in the Safe wallet.

### Why did you decide to build it

> I (Paul) often feel frustrated that I can't use Ethereum dapps on my mobile phone the way I would with any "web 2" app. For instance, sometimes I want to add someone to the Aragon DAO for my Meetup group on my phone while I'm talking to them at a meetup, but instead I have to set a reminder to do it when I'm back at my computer at home. I could do it within a dapp browser, but the UX of a webview inside of another app is clunky enough that I don't consider it as a realistic option. If I'm noticing this inconvenience as someone who's technical, the average potential Ethereum/dapp user surely feels that pain much more. The Ethereum community loses mainstream people from the onboarding funnel because of this.

> Young people use mobile devices way more than laptops, and the same is true in general for people worldwide - it feels very "centralized" of the Ethereum community to focus primarily on web-based dapp experiences on a laptop.

> About a year ago, I originally was interested in building an Ethereum dapp data explorer tool with simpler UX. Gradually, I realized that since my top priority is delighting mainstream users and introducing them to crypto and Ethereum (without them necessarily knowing that they’re using Ethereum), enabling developers to create mobile apps for using dapps would impact mainstream users far more than an exploratory tool. Talking to other people in the Ethereum community online and at conferences only strengthened this conviction and helped to refine the specifics of the idea.

### How long will it take

> We will need 3 months to ship version 1.0.0 of the project.

### How much funding are you requesting

> \$34000 _(Please see the timeline section for a detailed breakdown of the reasoning behind this number.)_

### How did you hear about the GECO

> Talking with Gnosis software engineers at Devcon4 in Prague

## Your Proposal

### Project description

##### A detailed description of your project

> One major reason most dapps don’t have standalone mobile apps today is because it’s harder for developers to build mobile Ethereum dapps than it is to build web-based dapps. There isn’t any good tooling for Ethereum in the React Native ecosystem. The Tasit SDK provides this. React Native is an especially great fit for mobile dapps since React is such a commonly used technology for web-based dapps - this allows for more code reuse. Moreover, many talented younger developers are opting to build their apps in React Native as opposed to Swift (for iOS) or Java (for Android) so that their app "automagically" works on both platforms.

> The 3 main source of UX friction this SDK addresses are:
> (A) Using a dapp within a web3-enabled browser dapp is an unacceptable UX. Almost all legitimate experiences on mobile today happen in standalone native apps.
> (B) As someone who already has ETH and tokens, needing to transfer some of these funds permanently from my preferred mobile wallet to another account in order to use a dapp is an unacceptable UX.
> (C) Needing ETH or tokens in the first place to try a dapp is too much onboarding friction.

> These problems can be solved with a JavaScript SDK for writing mobile apps for Ethereum dapps in React Native with a few advanced onboarding features built in. This helps developers build new mobile dapps more quickly without reinventing the wheel for basic features.

> Features

- Account and private key generation
- Reading and writing data and reacting to events
- Advanced support for popular ERC standards
- Onboarding
- Configurable JSON-RPC client
- Automatic scaffolding using the Tasit CLI

##### The overall goal and future outlook of your project

> Once the Tasit SDK is around, more dapps will have dedicated mobile apps. This will remove a key barrier to mainstream adoption of Ethereum dapps.

> Developers shouldn't need to reinvent the wheel for each new dapp: account and private key generation, linking to another wallet or adding meta-transaction support, etc. Let the Tasit SDK handle that bit and focus on the business logic for your dapp.

> In the future, we'll support the following based on demand:

- Serenity (eWASM, sharding, proof of stake)
- The Graph protocol
- State channels
- Plasma
- Future popular ERC standards
- In-app and/or singleton-on-device light and ultralight clients with a simple abstraction around them
- Use of upgradeable and nonupgradeable contracts
- Tool for finding the current address of a popular smart contract
- etc.

##### Why we should fund you.

> I (Paul) have a unique eye for product. I've shipped production mobile apps and worked with a team on an evolving JavaScript code base. I'm experienced with React Native and Ethereum. I've vetted the idea at conferences like Dappcon, TruffleCon, and Devcon4. Plus, people enjoy working with me.

> Tasit will serve as "proof of decentralization" for the dapps we support. Vitalik tweeted 'One simple litmus test for whether or not a blockchain project is truly decentralized: can a third party independently make a client for it, and do everything that the "official" client can?'. It's time for major decoupling of "back end" and front end. This decoupling provides users with "right to exit".

### Features

> _Note: There are more specifics on the features in the deliverables sections below._

##### Tools and frameworks

> ethers.js, React Native, Expo, Jest, Truffle, Babel, Infura, Lerna, smart-contract-based wallets (Gnosis Safe in particular), meta-transactions, ERC721, ERC165, Fastlane, CircleCI

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

> Paul recently worked on a smart contract audit for OpenZeppelin 2.0 with the team at Level K (plus a few other high-profile audits). For the past year and a half he has been working as a freelance software engineer specializing in Solidity, IPFS, Truffle, React, and React Native.

> He has a lot of experience working on native mobile apps, most recently including the Heatworks mobile app. Before that he was the first hire and CTO at the YC-backed IoT startup Edyn - he wrote the initial code for much of the tech stack (Node.js, AWS, mobile, etc.), and as CTO he led the growth of the software and data science teams to 12 people. The Edyn team shipped 10,000 units of their IoT products and continuously iterated on a production mobile app to use with them.

> _Education:_ He received a BSE from Princeton in Electrical Engineering in 2008, and he received his Master's degree from Harvard in Systems Biology in 2014.

##### Marcelo Morgado

[LinkedIn](https://www.linkedin.com/in/marcelo-morgado/) // [Medium](https://medium.com/@marcelomorgado) // [GitHub](https://github.com/marcelomorgado)

> Marcelo is a full-stack developer with >5 years of experience and a sysadmin with >10 years of experience. He has participated in and lead multiple software development projects. He is a cryptocurrencies, decentralization, and open-source enthusiast.

> Marcelo has personally faced the problem that we're trying to solve. He participated in a Status Hackathon in September 2018. The web app he built works and received the 2nd place award at the hackathon. However, the associated React Native mobile project still only is a prototype, because he didn't have enough time to build an Ethereum wallet from scratch and then build a dapp during the hackathon. He has been following crypto technologies for 4 years now, and he thinks that one of the greatest barrier to the mass adoption of crypto and dapps is the friction with handling private keys, identity, and gas.

> _Education_: He recently took a course on Digital Currencies (DFIN-511) at the University of Nicosia in Cyprus. In 2013, he received his bachelor's degree in Information Systems from PUC-RIO (the #1 Brazillian private university) in 2013.

### Timeline, Milestones and Deliverables

**Phase I - v0.1.0**

**Deliverables**

- Ephemeral account and private key generation

- Higher-level abstraction for reading and writing data and reacting to events

- Advanced support for ERC721

- Onboarding using the Gnosis Safe for users with funds in there already

- Proof-of-concept app for Decentraland on TestFlight for iOS on a testnet

**Time and Price Estimate**

> 1 month, \$16500 total

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

> 2 additional months, \$17500

- \$2000 design contract work

- $13500 1 month of $6,750/month pay for 2 software engineers (salary for the 3rd month to be secured from elsewhere)

- \$2000 travel to conferences to speak about the project and attract other developers to use and/or contribute to the SDK.

**Phase III**

> We have plans for phase III and beyond, but I'm intentionally keeping the scope of this initial grant request smaller.

### Other

- [Website](https://tasit.io/)

- [Twitter](https://twitter.com/tasitlabs)

- [Project Kanban board](https://github.com/orgs/tasitlabs/projects/1)

- [Telegram](https://t.me/tasitlabs)

- [Email](mailto:founders@tasit.io)

- [Feature requests](https://tasit.canny.io/feature-requests)

- [Here's a video](https://youtu.be/PPbwf1-4Jpk) of Paul Cowgill pitching Tasit Labs (the company doing most of the initial work on the Tasit SDK).
