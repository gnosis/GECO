## Project Overview

### Project name

Token registration and push 

### Team members 

Mikko Ohtamaa
Ville Sundell
Voith Mascarenhas

### What project are you building 

A protocol that allows the end user to register token entries in different wallets easily. 

### Why did you decide to build it 

Token and tokenised assets drive the decentralised finance ecosystem. When new users are onboarded, the first UX challenge is usually get and display different tokens in the wallet the user is having. The user wants to confirm they receive tokens sent to the user.

Currently all wallet providers manage default centralised token lists that their wallets support. This is not good as 1) centralisation and whitelisting is against the blockchain ethos 2) for a token issuer updating different token lists for wallets is very cumbersome.

We expect the number of tokens to grow thousands folds in the future. Managing good centralised list will be impossible. Thus, we propose a different solution. A way for the issuers to push and easily allow users to register tokens in their wallets when the user receives the tokens for the first time.

### How long will it take 

3-5 months.

### How much funding are you requesting  

$74,000

### How did you hear about the GECO

A personal relationship with Gnosis.

## Your Proposal 

### Project description

A protocol candidate and the first reference implementation to push token registrations with Gnosis SAFE wallet and one other wallet provider. 

### Features

- An ERC proposal for a token registrations

- A protocol to push a token registration over WalletConnect API 
  - If the user is using a decentralised service with WalletConnect, the service can registers the tokens needed for it in the user wallet 
- A protocol to push a token registration by scanning a QR code
  - Works with mobile wallets - the issuer published the registration QR code on their website 
- A protocol to push a token registration via URL handler or copy-paste 
  - A use case for MyEtherWallet like wallets 
  - A use case for a web browser plugin wallets
- A protocol to automatically register and show any tokens send to the user  
  - A mechanism against spam / airdrops to ensure random airdrops do not cause user distraction  
  - Reputation and fee based opt-in decentralised system for issuers and users to co-operate e.g. using GNO token
- An example project with HTML/JS for developers how to integrate this with their dApps and websites 


### Team description

All team members are on TokenMarket payroll. TokenMarket have issued out 30+ utility tokens and is now working with regulated security token issuances and security token decentralised exchange. We work with Python backend, JavaScript/React frontends.

### Timeline, Milestones and Deliverables

**Phase I: specification**

ERC proposal for the specifications 
- JSON format 
- WalletConnect changes needed  
- Gather feedback from Ethereum community with ERC process and asking in a person in meet ups and hackathlons 

**Time and Price Estimate**

1 working month 
$12,000

**Phase II: reference implementation with Gnosis SAFE **

**Deliverables**

A way to register tokens for the Gnosis SAFE user wallet using two different methods (e.g. WalletConnect or QR scan). 
- Browser plugin changes
- Mobile app changes (Android OR iOS)
- Server-side infrastructure changes (Gnosis SAFE WalletConnect)
An example HTML/JS application how to implement and test this 
A promotion of the example for Ethereum developer community. 

**Time and Price Estimate**

3 working months 
$36,000

**Phase III: from concept to robust implementation**

- Another mobile app support (Android OR iOS remaining)
- A decentralised system that allows user wallets to receive token registration without explicit action needed from the user, focused on good UX and spam protection

**Time and Price Estimate**

3 working months
$36,000 
 
### Others	 

TokenMarket is facing the challenge of having the securities token show up in the third party wallets. After dozens of issuances and working with multiple wallet providers, we believe we have the best experience can solve this problem by working with the wallet providers and other industry partners to solve this problem for the ecosystem as a whole. We also believe that Gnosis SAFE is a good candidate for the reference implementation, as all of their source code is open and Gnosis is open for co-operation. 

For another reference implementation, other than Gnosis SAFE wallet, we will open a dialogue with different wallet providers and see how would be likely to implement ERC.
