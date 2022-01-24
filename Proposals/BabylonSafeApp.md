## Project Overview

### Project name

> Babylon.finance

### Team members

> Tyler Murray, Ramón Recuero, Raúl Riesco, Igor Yalovoy, Sofi Vissani

### What project are you building

A platform for Crypto native investment clubs on ethereum. Individuals or communities can open a fund, deposit assets, submit investment strategies, and vote to determine the composition of fund. Investment gas costs are socialized through pooled capital. Successful strategies earn BABL (the protocol governance token) for LP’s, strategists, and voters relative to the weights set in fund.

Within the Gnosis eco system and beyond we want to become the go-to tool for managing treasury investments. As a first step this means adding a direct integration in the Gnosis Safe app catalogue.

### Why did you decide to build it

> It’s a tool we needed for ourselves and nothing quite fit our use case. All other asset management platforms on Ethereum L1/L2 platforms are repurposed TradFi implementations and we wanted a protocol that fit our world view for how a crypto native investment fund should work.

### How long will it take

> The core product is in Beta and live on Ethereum main net now.

> We expect the Alpha version of this Gnosis integration to take ~2-3 weeks of development time. It would consist of a wrapper around our core contracts with some minimal branding / UI. (Similar to the Compound application that offers limited but sufficient functionality)

> A full v1 that offers a deeper integration we expect to take up to another 4 weeks. This version would include the full suite of tools offered on Babylon in the Gnosis App and would allow for signature based transactions (greatly reduced tx gas costs) from contract wallets like Gnosis safe.

### How much funding are you requesting

> $35,000 USD for design, development, marketing of Alpha -> V1.0 and future improvements including but not limited to deeper integration of Gnosis Safe in Babylon’s ecosystem. ie: BABL token staking through Gnosis

### How did you hear about the GECO

> We use Gnosis Safe to manage our team and foundation treasuries and have colleagues / peers who work at Gnosis.

## Your Proposal

### Project description

We propose building a multi-phased implementation for Gnosis Safes to deposit / withdraw and otherwise interact directly with the Babylon.finance protocol. The mid-term goal is to seemlessly support management of sophisticated treasury investments for the largest DAO’s and investors using Gnosis Safe to secure their funds.

We already have interest from projects like Parsiq, Pickle StakeWise and others to manage their DAO treasuries in Babylon and a more formalized integration with Gnosis Safe could greatly expand the number of projects interested in managing treasury investments on Babylon.

### Features

Roughly the following features will be included:

1. Fund creation from Gnosis Safe
2. Asset flow
   a. Ingress / egress from Gnosis Safe (direct transaction)
   b. Signature based ingress / egress ([Sending gasless transactions - OpenZeppelin Docs](https://docs.openzeppelin.com/learn/sending-gasless-transactions))
3. Strategy Submission from Gnosis Safe
4. Strategy Voting from Gnosis Safe
5. BABL Staking from Gnosis Safe

Most of this functionality already exists and can easily be ported to a simple web GUI as a Gnosis App. Items 2a, 4, and 5 require signatures and thus would require some contract updates to support the style of signature implemented in the Gnosis Safe contract.

### Team description

The team has deep solidity and application development experience in Web2 / Web3. Past organizations include OpenZeppelin, Google, Looker, Moz and Allen Institute for AI. We have built and very sophisticated dApp and Protocol in less than one year that can be viewed here: https://www.babylon.finance

### Timeline, Milestones and Deliverables

Tentative multi-phase approach would look like the following:

**Phase I** Alpha Use Case

**Deliverables**
Simple port of 3 key features:
Garden (fund) creation, Garden property management, and asset ingress / egress directly from the Gnosis Safe application.

This unlocks a DAO to create a fund, add wallets that can participate in the submission and voting of strategies, and deposit / withdraw treasury funds from the Garden.

Key limitation here is that the DAO gnosis wallet would not be able to submit strategies or vote on them directly so that would require other wallets to do so on behalf of the DAO. This is supported by the DAO whitelisting addresses to participate in the Garden (fund).

**Time and Price Estimate**
2-3 weeks
$5,500 - $7,500 USD

**Phase II** Gnosis Signature Support

**Deliverables**
This phase would enable the Gnosis wallet to sign transactions (unlocks gasless ingress / egress, voting, and staking when available). This will creatly reduce the cost to manage the DAO's position and opens up direct management of the strategies of the fund by the DAO multi-sig if so desired.

**Time and Price Estimate**
2-4 weeks
$10,000 - $15,000 (requires Solidity development / mainnet deployment(s))

**Phase III** Full Application Support

This phase will likely replace the existing user experience because the functionality of features like submitting a strategy can be moderate to very complex and a simple UI port is not feasible at this stage. Likely an integration similar to dHedge or others that support a viewport like experience will be required. In this case all existing core features of Babylon will be supported in the Gnosis app.

**Deliverables**
Full Babylon support. This will include any claiming, or other token related actions. At this point a DAO can manage all aspects of their treasury investments through Babylon as well as participate in the governance of the Babylon protocol and the soon to be released staking mechanics for BABL holders.

**Time and Price Estimate**
2-3 weeks
$5,500 - $7,500 USD
