# WalletConnect Microgrant

 
One of our primary goals at Gnosis is to increase the usability of dapps which we believe will play a vital role in the widespread adoption of blockchain technology. Supporting projects that improve the decentralized application user experience will prove an essential contribution to Ethereum wallet infrastructure.
 
In an effort to improve the Safe’s dapp interoperability, we have decided to offer microgrants to teams that are interested in building a WalletConnect integration that is compatible with the Safe. WalletConnect is an open protocol that allows users to establish a secure connection between a decentralized application and mobile wallet by simply scanning a QR code. This makes connecting to and interacting with the Ethereum blockchain quick and painless. We are therefore big supporters of WalletConnect and recently released a WalletConnect integration with the Safe. 
Moving forward, the Gnosis Ecosystem Fund will provide microgrants to teams interested in creating a WalletConnect integration that is compatible with the Gnosis Safe We will support successful integrations with up to $3,000 in funding.

## How can I apply? 
At the end of each month, we will give out one grant, although teams can submit a proposal at any time. Please complete this document if you are interested in applying.

## How to submit your proposal
* Fork the WalletConnect microgrant repo
* Create a new file with your project’s name
* Outline your proposal in that file
* Create a Pull Request to merge your submission into our repository

## Is my project eligible? 
We will only consider projects with a user base who have not received funding from VCs or token sales.

## What functionalities do I need to deliver? 

The integration with the Safe through WalletConnect should have the following attributes: 

* **Supports WalletConnect** > v1.0.0 (i.e. not v0.7.x)
* **Compatible with the Safe**
   * The dapp should not use message signing
   * If you do use message signing, you need to build a workaround for the Safe (eg. Like the one done for Alchemy)
   * Teams can also work with us on a contract signature integration please note that this is not a live feature yet, but will be available on Android by DappCon (Aug 21st)
* **Runs on mainnet**
* **Visible WalletConnect integration**
   * The WalletConnect connection should be directly visible in the UI  e.g. https://web3connect.com/ 
* **Bridge server**
   * You should host your own bridge server or use the Gnosis bridge server hosted at https://safe-walletconnect.gnosis.io  

## Some final points...
The WalletConnect integration must be open source as well as your project.
You should create a screencast or video on how to use the Safe with your dapp via WalletConnect as shown in this example. 

## Additional Information: 
* Gnosis Safe WalletConnect integration: https://github.com/gnosis/wallet-connect-swift
* Blog Post: The Gnosis Safe Now Has a WalletConnect Integration!
* WalletConnect Docs: https://docs.walletconnect.org 
* Examples: https://walletconnect.org/apps  
