# Microgrant Application
_KnownOrigin.io_


### Dapp name
> KnownOrigin.io - http://knownorigin.io

### Team members
> James Morgan
> Andy Gray
> David Moore
> Oliver Carding

### GitHub Repo
> https://github.com/knownorigin

### What is your Dapp about?
> KnownOrigin.io provides a platform for artists and creative to showcase and sell digital arts.
> Artists can create multi-edition artworks which are backed by non-fungible tokens, NFTs. (ERC-721 compliant) 
> Users can browser and find rare digital artworks, placing bids or buying the artwork at list price.

### Why did you decide to build it?
> Originally design to compliment a physical popup art gallery in April 2018, it has morphed from a fully administered
platform to one which allows on-boarded artists, currently 126, to create and manage their own works.
> We also believe that NFTs can provide an enhanced solution to properties such as ownership, authenticity and provenance.  

### How big is your user base?
> Since launch our high level platform stats are as follows: (17th Aug 2019)
- Total NFTs sold - 2728
- Total number of NFTs available - 9198
- Total editions - 716
- Total artists - 126
- Total ETH raised (primary & secondary sales) - 94.36 ETH
- Total onchain txs, last 30 days - approx 420 
- Avg daily users, last 30 days (Google Analytics) - approx 60-100

### How long will you need to integrate a Gnosis Safe compatible WalletConnect integration?
> I have not looked to closely into whats required but I think I will need approx 2-3 weeks to fit in the dev time to integrate Gnosis safe and enable wallet connect.

### Does your Dapp use message signing?
> Yes, unfortunately we use message signing for two things:
 - When a user has purchased some of the older editions we ask them to sign a txs to confirm ownership before giving them access to a high-res version of the artwork. This is only a problem on historic items. 
   To mitigate this risk I can switch the process when Gnosis safe is being used to provide a direct download link. 
 - We also use txs signing to confirm actions a artists whats to make to off-chain data e.g. profile updates. I dont think will be an issue as all artists are currently onboarded using MM or mobile wallets like Trust or Cooinbase wallet. 
 
### How did you hear about the GECO?
> Twitter

### Others
> It has been on my list to integrate wallet connect for a while now. I think the combination of Gnosis safe and Wallet connect can provide a solid solution for our users. 
 - In the future I want to investigate how things like meta-txs can be leveraged on KnownOrigin as well as some of the other dapps we build. 
 - The company which maintains and builds KnownOrigin is http://blockrocket.tech - I think that adding to KO will provide a good level of understand for us to then consider
   and be able to add it for our other dapps as well as offering it to clients of ours who ask us to build dapps for us. 
   
