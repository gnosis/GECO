# Proposal Guideline

## Project Overview

### Project name

Pooltogether

### Team members

Me :D
@denhampreen

(& @konradhugo (Recent grad that wants to learn more about blockchain))

### What project are you building

I want to build an integration with [pooltogether](https://pooltogether.com).

### Why did you decide to build it

I came across this grant program a while back and thought it a really cool way to build some fun tech and get compensated while doing it!

I have grander visions of building more integrations, such as tornado cash, but thought Pooltogether would be a good entry level and useful application that Konrad can learn with too.

Pooltogether is beautifully simple and an application I believe is some what of a bridge for the non crypto world 🤓.

From what I have seen there is no pooltogether integration yet.

Gnosis safe although often positioned towards custoding company funds, is my go to recommendation for securing & holding larger amounts of crypto to my friends and family because of it's inherent properties of recoverability and security (Having a mobile and desktop wallet with minimum 2 signers is the crypto equivalent of 2fa to me 😅).

Konrad wants to learn about blockchain and I believe this is a great way for him to get his hands into some usable applicable blockchain tech.

Disclaimer: We have no affiliation with Pooltogether

### How long will it take

2 weeks. I have looked at a few different safe app repo's, resources, German's yt video and pooltogether's gh and docs and believe it's a quite a straight forward integration.

### How much funding are you requesting

1500 DAI

### How did you hear about the GECO

I think Auryn originally🤷🏼‍♂️, maybe through looking at the docs a while back.

## Your Proposal

### Project description

The integration will allow safe owners to interact with the pooltogether contracts in the following way(s);

## Deposit flow

Pre deposited user

1. View pools (currently dai & uni)
   - Prize amount
   - Prize giving timeframe & prize round number
   - Countdown until next pool prize
1. Select pool
1. Set amount (max)
1. Approve token spend tx\* (set amount || unlimited)
1. Deposit tx

## Withdraw flow

Post deposited user

1. View active deposits (amount, how long, pool)
1. Withdraw deposit position

> \* New pooltogether contracts look like they allow permitAndDeposit (worth looking at closer better ux)

All aspects of the development will be documented with the intention of writing a medium article with a 'wiki' on how to we built the integration with the intention that other developers can explore developing FE in blockchain environment.

### Features

- Figma design mockup
- React (safe-app-cra-template)
- Hooks (safe-apps-react-sdk)
- Gnosis story book lib (https://components.gnosis-safe.io)

### Team description

@denhampreen
I work with 2 friends (@jasoons & @moose-code) on Wildcards.world. I have been working with react predominantly over the last few years.

Konrad is new to everything 😂. The project delivery and code quality will be ensured by @denhampreen

### Timeline, Milestones and Deliverables

**Phase I** _Design and Research_

**Deliverables** _Figma mock up, cra boilerplate, resource list_

**Time and Price Estimate** _4 days_

**Phase II** _Implementation_

**Deliverables** _Deposit flow & Withdraw flow_

**Time and Price Estimate** _10 days: 1500DAI_

### Others

Anything else you want to share with us -
[https://youtu.be/dQw4w9WgXcQ](https://youtu.be/dQw4w9WgXcQ)
