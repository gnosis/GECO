# Project Overview

## Project name

Aragon futarchy

### Team members

- Federico Luzzi ([Github profile](github.com/luzzif))

### What project are you building

An Aragon app to empower DAOs decision-making processes through futarchy.

### Why did you decide to build it

I first participated in the Fork the World hackathon with an Aragon prediction
markets app. The original idea was to help all DAOs (or at least Aragon-based
ones) to make better decisions through the use of prediction markets (where one
really has to put money where their mouth is, in order to express their thought
on a governance matter).

The project was soon to be reduced in ambition though, due to the scarcity of
time at my disposal, and due to the fact that I decided to develop it alone,
without a proper team (i.e. I actually underestimated the effort that I had to
put in).

Now that time constraints are not much of a problem (even though they're still
there), I'd like to expand on the ideas that I originarily had for the project,
and give Aragon DAOs a full-blown futarchy app.

### How long will it take

Probably not less than 2, or even 3 months (so, pretty much ETA would be by the
end of the year).

### How much funding are you requesting

4800 USD.

### How did you hear about the GECO

After winning the Fork the World hackathon with a reduced version of the to-be
project, Graeme Barnes contacted me to give me the possibility to expand on my
work through the GECO program.

## Your Proposal

### Project description

As I previously said, the end goal is to give Aragon DAOs the possibility to
carry on governance duties through futarchy, by setting up prediction markets
allowing to carry out specific actions (treasury funds unlocking,
DAO-proprietary token minting, recruitment and more) when a given market
resolves with a certain outcome, exploiting the tight Aragon's ecosystem.

### Features

Aragon apps are implemented using Aragon OS on the blockchain contract side, and
Aragon UI on the frontend side, exploiting event sourcing to get data from the
blockchain and display it to the user, producing an overall smooth experience.

### Team description

I'm a one-man-team. My dream has always been (at least from the beginning of
2017, when I first got to know BTC) to work in the crypto-space, and during the
COVID pandemic, I decided it was finally time to give it a real go. I
participated in a Loopring bounty on Gitcoin which had the goal to build them a
new, shiny frontend for their Loopring Pay protocol and won it, and shortly
after I enrolled in the Fork the World hackathon with my Aragon prediction
markets app, winning it as well.

From that point on it's all been incredible. The work produced on my first
bounty has now been carried forward by me and the dxDAO and has become Rails,
a webapp for fast, secure and gasless crypto micropayments ran through the
Loopring Pay protocol. You can test out the project and see what it's all
about (even on the Goerli testnet if you want) [here](https://dxdao-rails.netlify.app).

Since Loopring was pretty impressed with the frontend I built for them they then
contacted me to develop an Uniswap-like interface for their currently order-book
based dex (with the goal to abstract the order-book complexity away from the
user, improving the UX in turn). It's recently been released, and yo can find
it [here](https://swap.loopring.io)

### Timeline, Milestones and Deliverables

**Phase I**: Make users actually own the conditional tokens they trade.

**Deliverables**: Right now, when an user buys a given conditional tokens, they
don't own it. That's because everything is governed by the Aragon app's
contract, which owns all the tokens and keeps track of which parties own how
many and which tokens. This is obviously bad, since as a user, I'd want to have
my own tokens in my own wallet. The current approach is both error-prone (it
adds unnecessary logic to the SC) and not particularly secure (a severe bug in
the SC code could make a malicious actor get ALL the tokens, for example).

**Time and Price Estimate**: roughly 1 week, at a price of 800 USD.

---

**Phase II**: integrate a proper independent and decentralized oracle to
determine market outcomes.

**Deliverables**: right now, the market's creator can close the market whenever
he wants and choose whichever outcome he wants, even maliciously (this was done
to have a PoC for the app, due to the lack of time). The goal here is to use
Realit.io and Kleros to determine correct market outcomes in a fair way. The
approach will be very similar and inspired from the one Omen uses today.

**Time and Price Estimate**: roughly 2 weeks, at a price of 1600 USD

---

**Phase III**: make use of every possible ERC20 token as collateral.

**Deliverables**: right now, only WETH is supported as a market collateral (and
even worse, it is supplied as raw Ether when collateralizing a market and
returned as wrapped Ether when redeeming positions, which clearly has to be
fixed). The goal here is to make it possible for a market creator to
collateralize a market with any ERC20 token at their disposal (even the DAOs
proprietary token).

**Time and Price Estimate**: roughly 1 week, at a price of 800 USD

---

**Phase IV**: integrate with other Aragon apps.

**Deliverables**: the goal here is to make the app what in Aragon is called a
forwarder, by effectively being able to attach EVM scripts to the creation of a
given market and execute them only if the market resolves with a certain
outcome.

**Time and Price Estimate**: roughly 4 weeks, at a price of 1600 USD
