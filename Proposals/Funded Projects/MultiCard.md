## Project Overview

### Project name
MultiCard

### Team members
Dietmar Hofer, Peter Grassberger, Thomas Haller (all members of [lab10 collective](https://lab10.coop))

### What project are you building
We want to build an MVP which allows holders of [Blockchain Security 2Go smart cards](https://github.com/infineon/blockchain) to sign Safe transactions with a Raspberry Pi connected NFC reader.

### Why did you decide to build it 
This NFC smard cards combine high safety and usability. They encapsulate the private key and make signing transactions as easy as scanning the card with an NFC reader.  
The lack of a way to backup the private key is a big issue for many conventional use cases. But this issue can be mitigated by using such keys as key shares of a multisig.  

We believe that using such smard cards in combination with Gnosis Safe unlocks many interesting use cases, thus we want to explore that, starting with an MVP.

### How long will it take 
We plan to have a nice MVP in one month.

### How much funding are you requesting  
We're requesting the minimal amount of 5k $.

### How did you hear about the GECO
A lab10 team member told me about it a few hours before the first submission deadline.

## Your Proposal 
### Project description
The MultiCard MVP will consist of 
* a setup module which allows to initiate cards as key holders for a Safe contract
* a simple UI which allows to initiate Safe transactions and shows the state of that transaction (e.g. process of collecting signatures, lifecycle of the wrapping Ethereum tx)
* a background process which handles NFC communication with the cards and communication with the Gnosis Safe contracts

We already had an opportunity to get hands-on with this smart cards at a Hackathon hosted in the context of its first public release ([link](https://letscluster.com/infineon-hackathon/)). In the context of this Hackathon we also started studying the Gnosis Safe contract system and got intrigued about the possibilities it opens up.  
At lab10 we are also working on the concept and initial implementation of [Minerva - a digital wallet](https://lab10.coop/en/projects/minerva) for identities, valuables and credentials.  

This MVP is intended to help us explore and understand the best ways to build easy to use and easy to explain/understand applications and systems which are needed in order to unlock the advantages of decentralized systems to a larger audience. This could for example be a backup/recovery mechanisms for the Minerva wallet, or standalone applications which solve very specific problems (e.g. use cases which nowadays still require paper to travel around in order to collect ink signatures).

### Features
We plan to implement the MVP as a node.js / web application which will of course be released as open source.

### Team description
* [Dietmar Hofer](https://github.com/d10r) dived into Ethereum in 2016, learning blockchain basics [by implementing one](https://github.com/d10r/l10chain), likes to explore [what else could be done](https://github.com/lab10-coop/streem-poc).
* [Peter Grassberger](https://github.com/PeterTheOne) is an avowing [pirate](https://www.piratenpartei.at/) who actively defends our freedom and privacy in the digital space. He already wrote several Dapps at lab10.  
* [Thomas Haller](https://github.com/SurfingNerd) likes surfing and gaming, in between he also maintains the governance Dapps and Explorer of the [ARTIS blockchain](https://artis.eco) (a lab10 initiated Ethereum sidechain).
