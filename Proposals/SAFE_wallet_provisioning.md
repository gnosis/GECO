## Project Overview

### Project name

SAFE wallet provisioning

### Team members

Mikko Ohtamaa
Alexander Smith
Rainer Koirikivi

### What project are you building

An automated wallet provisioning for new users for decentralised finance services.

### Why did you decide to build it

TokenMarket, a security token marketplace, is facing the problem that it is too difficult for non-tech-savvy users to get a secure blockchain wallet installed for themselves.

To participate the decentralised finance, the users first need to have a wallet. Furthermore they need to have loaded it with some cryptocurrency and tokens to make it useful. There is a lot of separate steps to get the wallet in the hands of the user.

This problem is also described on this slide from https://pbs.twimg.com/media/D1C-p3WWwAUuyWv.jpg

We want to make the process smoother for the end user. For new users, we assume they come through a website, with their normal web browser. We want to streamline the experience, so that the users can get a secure, mobile based, wallet in their hands with minimal amount of clicks.

### How long will it take

3-5 months.

### How much funding are you requesting  

$74,000

### How did you hear about the GECO

A personal relationship with Gnosis.

## Your Proposal

### Project description

Gnosis SAFE wallet automated installer for decentralised finance application vendors.

We assume that the best way to make new users to want to install a wallet is through a service that they want to use and they need a wallet for it: install the wallet when it is required for the first time.

The users, who do not have a wallet yet, are prompted to install one on a website. The process starts by asking a mobile phone number from the users. After entering the mobile phone number, we send an SMS link to Gnosis SAFE installation (iOS/Android). 

After the user installs the app, and the seed phrase is safely set up, a backend service receives a notification about the installation. 

The original vendor, from whom the installation request came from, receives a notification that the user has now successfully installed a wallet. 

If the finance application vendor chooses so, they can also pay the initial fees for the user (ETH seed money) and transfer any other finance application specific tokens to the user wallet. 

The vendor can automatically whitelist the new address of the user in their service, the wallet is automatically WalletConnect'ed and also push the user any token registration needed in order to use the service.

Ultimately, the wallet adoption process should take only four steps from the user point of view
1. Enter your phone number on a website that needs the wallet
2. Click a link in the SMS that takes you the appropriate app store purchase page 
3. Install the wallet app
4. Choose a seed phrase backup option
(5.) The service is now aware that the user has a working wallet in their hands

### Features

- A wallet installation module for a website 
  - An IFRAME integration on any website 
  - Asks for a phone number and sends the relevant app installation SMS 
  - Tracks the installation id, so that the after the wallet installation we can trigger a webhook notification 
  - Either hosted within Gnosis SAFE server side infrastructure or a (self hosted) standalone server side Python application  
  - Spam protection e.g. through API key and deposit or similar  

- Alternative installation mechanism (not SMS)
  - Scan a tagged QR link, with a vendor generated tag, which takes user to the app store installation page
  - E.g. for Asian audience where QR code method may be more prevalent 

- A vendor payment service
  - Pay the installation of the wallets on behalf of the user 
  - Pay the initial ETH fees on the behalf of the users 
  - Also load any other tokens in the wallet 
  - Potentially using GNO token

- Automated registration of tokens in the new wallet installations  
  - When a wallet is installed, make sure the relevant tokens needed for the vendor service show up in the wallet 

### Team description

All team members are on TokenMarket payroll. TokenMarket have issued out 30+ utility tokens and is now working with regulated security token issuances and security token decentralised exchange. We work with Python backend, JavaScript/React frontends.

### Timeline, Milestones and Deliverables

**Phase I: specification**

A proposal for changes in Gnosis SAFE architecture in order to have the streamlined installation flow 
- Mobile user experience changes needed
- SMS gateway - who will operate it and how to pay the SMS gees 
- How to serve IFRAME for phone number input
- How the vendor receive a notification after the user has successfully installed SAFE wallet 
- Privacy concerns and how to address them 
- Integration to the other components of SAFE architecture, like coupons or referral fees
- How to automatically set up WalletConnect for the installed wallet

**Time and Price Estimate**

1 working month
$12,000

**Phase II: minimal viable product (MVP)**

**Deliverables**

An alpha version of Gnosis SAFE where the installation flow is supported.

- Mobile app changes in one ecosystem (either Android OR iOS)
- Server-side code changes 
- An SMS gateway set up 
- A vendor notification webhook / polling API endpoint set up
- An example HTML/JS application how to implement and test this
- A ready to be published in the app store, but the features hidden from the end user
- Present the service in relevant Ethereum meetups

**Time and Price Estimate**

3 working months
$36,000

**Phase III: beta implementation and vendor tooling**

- Another mobile ecosystem supported (Android OR iOS remaining)
- A vendor dashboard 
  - Receive your API key, either through website sign up or a smart contract transaction sign up
  - Vendors can self sign up for the service 
  - A vendor have a dashboard to have visibility to Gnosis SAFE flow (number of installs, countries, users currently stuck in the pipeline)
- Gnosis SAFE dashboard 
  - Number of vendors signed up
  - Total installations the vendors have driven for SAFE 
  - Best performing vendors
  - Enable/disable vendors in the case of manual troubleshooting 
- Polished developer documentation 
- Present the service in relevant Ethereum meetups

**Time and Price Estimate**

3 working months
$36,000

### Others	 

TokenMarket is facing the challenge of having the user to install wallets. After dozens of issuances and working with multiple wallet providers, we believe we have the best experience can solve this problem by working with the wallet providers. We also believe that Gnosis SAFE is a good candidate for pushing the envelope in this matter, as all of their source code is open and Gnosis is open for co-operation.

We have also worked in the past with the www.linktexting.com that solves this problem for mobile apps in a generic manner, but lacks the necessary bits for the cryptocurrency integration and vendor callbacks to inform when the wallet is ready for the action.
