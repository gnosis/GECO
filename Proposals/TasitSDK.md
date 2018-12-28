# Proposal Guideline

_This is a guideline on how to best structure your proposal._

## Project Overview

### Project name

> Tasit SDK

### Team members

> Paul Cowgill, Marcelo Morgado

### What project are you building

> The Tasit SDK is a JavaScript SDK for making standalone native mobile Ethereum dapps using React Native.

Here's a video of Paul Cowgill pitching Tasit Labs (the company doing most of the initial work on the Tasit SDK): https://youtu.be/PPbwf1-4Jpk

### Why did you decide to build it

> I often feel frustrated that I can't use Ethereum dapps on my mobile phone the way I would with any "web 2" app. For instance, sometimes I want to add someone to the Aragon DAO for my meetup group on my phone when I meet them at a meetup, but instead I have to set a reminder to do it when I'm back at my computer at home. If I'm noticing this inconvenience as someone who's technical, the average potential user must feel that pain even more. The Ethereum community loses mainstream people from the onboarding funnel because of this.

The 3 main source of friction are:
A) Using a dapp within a browser dapp is an unacceptable UX. Almost all legitimate experiences on mobile today happen in standalone native apps.
B) As someone who already has ETH and tokens, needing to transfer some of these funds permanently from my preferred mobile wallet to another account in order to use a dapp is an unacceptable UX.
C) Needing ETH or tokens in the first place to try a dapp is too much onboarding friction.

These problems can be solved with a JavaScript SDK for writing mobile apps for Ethereum dapps in React Native with a few advanced onboarding features built in. This helps developers build new mobile dapps more quickly without reinventing the wheel for basic features.

### How long will it take

> We will need 3 months to ship version 1.0.0 of the project.

### How much funding are you requesting

> \$34000

### How did you hear about the GECO

> Devcon4

## Your Proposal

### Project description

##### A detailed description of your project

##### Why you chose to build this project

See the section on why above. Also:
https://github.com/tasitlabs/TasitSDK/blob/develop/README.md#why

##### The overall goal and future outlook of your project

##### Why we should fund you.

React Native is an especially great fit for mobile dapps since React is such a commonly used technology for web-based dapps - this allows for more code reuse.

### Features

##### Tools and frameworks

ethers.js
React Native
Expo
Jest
Truffle
Babel
Infura
Lerna
Smart-contract-based identity (like Gnosis Safe)
Meta-transactions
ERC721
ERC165
Fastlane
CircleCI

##### Architecture, mockups, etc.

- [Architecture](https://www.dropbox.com/s/gw88c5ua4ssthvg/TasitProjectStructure.png?dl=0)

- A README with [more details on the Tasit SDK](https://github.com/tasitlabs/TasitSDK/blob/develop/README.md)

- A README with [more details on the Tasit apps](https://github.com/tasitlabs/tasit/blob/develop/README.md) - all the mainstream-user-facing apps for popular web-based dapps (like Decentraland, Aragon, etc.) that will be built using the Tasit SDK

- [Slides about the Tasit SDK](https://bit.ly/2018-12-04-chicago-ethereum-meetup)

- [Example app onboarding flow](https://youtu.be/iJQtDPQrRsE) (interactive wireframes)

### Team description

_Who are your team members, what is your background and what you built before._
Paul Cowgill
I recently worked on a smart contract audit for OpenZeppelin 2.0 with the team at Level K (plus a few other high-profile audits). For the past year and a half I've been working as a freelance software engineer specializing in Solidity, IPFS, Truffle, React, and React Native.

I have a lot of experience working on native mobile apps, most recently including the Heatworks mobile app. Before that I was first hire and CTO at the YC-backed IoT startup Edyn - I wrote the initial code for much of our tech stack (Node.js, AWS, mobile, etc.), and as CTO I led the growth of the software and data science teams to 12 people. We shipped 10,000 units of our IoT products and continuously iterated on a production mobile app to use with them.

Education: I did my undergrad at Princeton in Electrical Engineering, and my masters at Harvard in Systems Biology.

Marcelo Morgado

<!-- TODO: Add me -->

### Timeline, Milestones and Deliverables

**Phase I** v0.1.0

**Deliverables**

- Ephemeral account and private key generation

- Higher-level abstraction for reading and writing data and reacting to events

- Advanced support for ERC721

- Onboarding using the Gnosis Safe

**Time and Price Estimate**
1 month, $16500
\$2000 design contract work

$13500 1 month of $6,750/month pay for 2 software engineers

\$500 SAAS costs, like an Apple Developer Program account to have a test implementation of an app using the SDK, etc.

\$500 legal costs with Stripe Atlas

**Phase II** v1.0.0
Advanced support for DAOs, TCRs, or two-sided marketplaces.

**Deliverables**

<!-- TODO: Add me -->

**Time and Price Estimate**
2 additional months, \$17500

\$2000 design contract work

$13500 1 month of $6,750/month pay for 2 software engineers (salary for the 3rd month to be secured from elsewhere)

\$2000 travel to conferences to speak about the project and attract other developers to use and/or contribute to the SDK.

**Phase III**
We have plans for phase III and beyond, but I'm intentionally keeping the scope of this initial grant request smaller.

### Other

n/a
