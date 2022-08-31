# Microgrant Application
_KnownOrigin.io_

### Dapp name
> KnownOrigin.io - http://knownorigin.io

### Team members
> James Morgan - Fullstack/Blockchain engineer

> Andy Gray - Fullstack/Blockchain engineer

> David Moore - UX specialist 

> Oliver Carding - Marketing and strategy specialist

### GitHub Repo
> https://github.com/knownorigin

### What is your Dapp about?
> KnownOrigin.io provides a platform for artists and creative to showcase and sell digital arts.

> Artists can create multi-edition artworks which are backed by non-fungible tokens, NFTs. (ERC-721 compliant) 

> Users can browse and find rare digital artworks, placing bids or buying the artwork at list price.

> KnownOrigin is aiming to the go to place to buy trusted rare digital arts as well as providing 
a marketplace and social platform fit for the decentralised movement.

### Why did you decide to build it?
> Originally design to compliment a physical popup art gallery held in Manchester, UK in April 2018, 
it has morphed from a fully administered platform to one which allows on-boarded artists, currently 126, 
to create and manage their own works.

> We also believe that NFTs can provide an enhanced solution to properties such as ownership, 
authenticity and provenance.

### How big is your user base?
> Since launch our high level platform stats are as follows: (as of 27th Aug 2019)

- Total NFTs sold - 2947️
- Total number of NFTs available - 9915
- Total editions - 818
- Total artists - 126
- Total ETH raised (primary & secondary sales) - 100.94 ETH
- Total onchain txs, last 30 days - approx 400 
- Total users, last 28 days (Google Analytics) - approx 1700
- New users, last 28 days (Google Analytics) - approx 1400

### How long will you need to integrate a Gnosis Safe compatible WalletConnect integration?
> I estimate I will need approx 1-2 weeks to fit in the dev time plus UX changes required to integrate Gnosis safe and enable wallet connect.

> Our frontend is built in VueJs, I have seen a react component for Gnosis Safe so maybe at the end we will be able 
to release an official VueJS library as well.

### Does your Dapp use message signing?
> Yes, we use message signing for two things which I believe would not be impacted:

1) When a user has purchased some of the older editions we ask them to sign a txs to confirm ownership before giving them access to a high-res version of the artwork. This is only a problem on historic items. 
   To mitigate this risk I can switch the process when Gnosis safe is being used to provide a direct download link. 

2) We also use txs signing to confirm actions a artists whats to make to off-chain data e.g. profile updates. I dont think will be an issue as all artists are currently onboarded using MM or mobile wallets like Trust or Cooinbase wallet. 
 
### How did you hear about the GECO?
> Twitter

### Others
> It has been on my list to integrate wallet connect for a while now. I think the combination of Gnosis safe 
and Wallet connect can provide a solid solution for our users. 

> In the future I want to investigate how things like meta-txs can be leveraged on KnownOrigin as well as some 
of the other dapps we build. 

> The company which maintains and builds KnownOrigin is https://blockrocket.tech - I think that adding to KO will 
provide a good level of understand for us to then consider and be able to add it for our other dapps as well as 
offering it to clients of ours who ask us to build dapps for us. 
   
