
## Linkdrop Protocol

### Team members 

Mikhail Dobrokhvalov,
Dev lead,
https://github.com/Dobrokhvalov

Gustav Friis,
Biz lead,
https://www.linkedin.com/in/gustav-friis-20201086/

Artyom Ignatyev,
Product lead,
https://www.linkedin.com/in/artyomignatyev

Amirkhon Jumaniyazov,
Backend dev,
https://github.com/amiromayer

Haz,
Frontend dev,
https://github.com/spacehaz


### What project are you building 

**General description**

[Linkdrop](https://linkdrop.org/) is an open protocol for including digital assets and onboarding properties into links and QR codes. 
This allows non-crypto users to simply click a URL or scan a linkdrop QR code to get onboarded. Place check out our already live [mainnet demo applications](https://linkdrop.org/demo/) to see how this looks like for one-to-many and one-to-one linkdrops.

**GECO specific**

We wish to developer a full meta-linkdrop implementation in order to extend linkdrop functionality to Gnosis Safe

### Why did you decide to build it 

Our general motivation for working on the Linkdrop Protocol is that we see usability of web3 being a major blocker for mainstream adoption in an equivalent manner to scalability.
We see a meta-linkdrop module is a very useful feature to include in the wallet contract of the Gnosis Safe to seamlessly allow referral programs and invitation schemes to onboard new users.

### How long will it take 

The entire  [linkdrop protocol roadmap](https://github.com/LinkdropProtocol/Proposal-Paper/blob/master/README.md) spands for a year. The specific meta-linkdrop implementation is estimated to spand over Q2 and Q3 of 2019.

### How much funding are you requesting  
We are requesting $50.000 to develop the generalized meta-linkdrop SDK as well as and provide an end-to-end working solution for the Gnosis Safe

### How did you hear about the GECO

Through whispers in the full node office

## Your Proposal 
### Project description

**Regular linkdrops**

In our existing mainnet dapp implementations such as [eth2.io](https://eth2.io/) (one-to-one linkdrops) and volca (https://volca.tech/) (one-to-many linkdrops) a regular external Ethereum account is used.

**Meta linkdrops**

A meta-linkdrop is based on meta-tx accounts.That means that instead of working with an external Ethereum account, a meta-linkdrop works with digital asset stored in wallet contracts, such as Gnosis Safe and Universal Login based wallets.
This will be working quite similiar to this PoC of a [gassless webwallet utilizing Universal Login SDK](https://github.com/LinkdropProtocol/Gasless-Webwallet) we have recently built 

Our goal for this proposal is to make linkdrops work with the Gnosis Safe end-to-end, as well as deliver a generalized meta-link SDK implementation that other developers can use to integrate interoperable meta-linkdrops into their projects.


### An example of meta-linkdrop including Universal Login, ENS, ERC20 and ERC721 

![invite scheme](https://user-images.githubusercontent.com/18598519/48316096-10f8ab00-e5df-11e8-89f0-63a0397c904c.png)

1. Alice shares an invite link or QR code with Bob, including a transit private key and a signature
1. Clicking the link, Bob is directed to a webpage
2. Bob generates his own private key stored in the browser
3. Bob uses the transit private key to sign Bob’s address
4. Bob’s browser sends his two signatures to the relayer 
5. The Relayer calls Alice’s identity contract
6. Then Alice’s identity contract creates an identity contract for Bob and sends a Robot
7. In addition, Bob can now also help Alice recover access to her identity contract in the future using a social key recovery mechanism
8. Bob now got the Robot he wanted, and in addition has a Universal Login Contract and ENS name which allows him to use the best of web3 to login to all other Ethereum dapps.

### Underlying Assumptions

In order for the invite functionality scheme to work in practice, the following assumptions needs to be valid: 

- Alice has an EIP 1078 identity contract and wants to send an ERC721 or ERC20 token to Bob
- Bob is a new user without ETH, wallet or any prior crypto knowledge
- Alice share the QR code or invite link with Bob over a secure channel e.g Signal
- There is a proper incentive in place (on a user, dapp or relay level) to pay gas


### Team description

1. Most of us intially met at the Status Hackathon before Devcon 4 where we won two first prizes, for building the [onbotting.eth webapp](https://www.youtube.com/watch?v=K67dOixMBWI&t=). Prior to that tha Mikhail and Aritom had develped earlier versions of eth2.io and Volca 
2. Since then we together created the [cryptoxmas.xyz NFT charity](https://cryptoxmas.xyz/) and raised roughly 18 ETH to Venezuelans utilizing linkdrops and a Giveth campaign.
3. We have now developed the gasless-webwallet, and began on our roadmap to generalize the linkdrop protocol. 

We described [a bit about us and our story](https://medium.com/@Gfriiis/linkdrops-an-open-source-standard-for-invite-digital-asset-links-on-ethereum-29f34b3fa5ec) in this blogpost


### Timeline, Milestones and Deliverables


- Q2: Meta-linkdrop module to Gnosis Safe Contracts, estimated $15.000

- Q2: Relay implementation, assumed to extending on existing Gnosis backend, estimated $10.000

- Q3: Meta-Linkdrop SDK, estimated $15.000 

- Q3: Front-end Javascript libraries, estimated $10.000 

### Existing Codebase

https://github.com/LinkdropProtocol
