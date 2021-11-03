# Proposal Guideline 
_This is a guideline on how to best structure your proposal._

## Project Overview

### Project name
> Name of your project

Forta Agent Development by Arbitrary Execution

### Team members 
> Name your team members

Philip Gillett: philip@arbitraryexecution.com
Alexis Williams: alexis@arbitraryexecution.com
Jasper Clark: jasper@arbitraryexecution.com

contact:
Michael Hatton: michael@arbitraryexecution.com

### What project are you building 
> Short summary/abstract of your project

AE is requesting a grant to develop a suite of monitoring agents on the Forta Network for the Ethereum. 

Forta is the first decentralized runtime security network for smart contracts. The goal of Forta is to detect threats and other system critical issues as soon as possible. By providing users with timely and useful information about the security and stability of their systems, they have an opportunity to react and take defensive action, preventing or minimizing loss of funds.  

The Forta Network has two main components - agents and nodes. Agents are pieces of logic (scripts) that look for certain transaction characteristics or state changes on smart contracts across any Layer 1, Layer 2, or sidechain. Nodes run agents against each mined block of transactions. When the agents detect a specific condition or event, the network emits an alert which is stored on IPFS and linked on a public blockchain. Forta will also maintain an automated public registry of all alerts, and anyone interested in the security of a contract can consume relevant alerts via the Forta Explorer Web UI or through the Forta API. 

### Why did you decide to build it 
> Short summary of your motivation 

We believe a decentralized runtime security network is a critical component of a global, open financial system. Whereas security audits focus on pre-launch vulnerability detection in smart contract code, Forta will actively monitor protocol activity post-launch and generate important alerts. 

We believe the value of Forta is to prevent and/or mitigate the impact of malicious activity, and generally have better visibility over your system’s health and performance, and the health and performance of other third-party contracts you rely on.

### How long will it take 
> Estimation of how long you will need to finalize the project

We anticipate three weeks to develop six Forta Agents.

### How much funding are you requesting  
> How much money do will you need to finalize the project

$30,000

### How did you hear about the GECO
> Website, Twitter, Conference and others

https://www.defigrants.org

## Your Proposal 
### Project description
_Outline a detailed description of your project, why you chose to build this project, the overall goal and future outlook of your project and why we should fund you._

The Forta Network has two main components - agents and nodes. Agents are pieces of logic (scripts) that look for certain transaction characteristics or state changes on smart contracts across any Layer 1, Layer 2, or sidechain. Nodes run agents against each mined block of transactions. When the agents detect a specific condition or event, the network emits an alert which is stored on IPFS and linked on a public blockchain. Forta will also maintain an automated public registry of all alerts, and anyone interested in the security of a contract can consume relevant alerts via the Forta Explorer Web UI or through the Forta API. 

As part of this project we would like to first discuss which agents would be most useful for the Gnosis team. Below is a sample list of agents that we have created and proposed to various blockchain protocols. The list below can be used as examples on what can be done. We make the behaviors configurable so that the protocol owners can adjust thresholds and other parameters to make them more or less sensitive.

Agents:

Governance and Admin Events
     Monitor events emitted from smart contracts.  The monitored events are settable through JSON file.

Pool Creation
    Identify when new liquidity pools are created

Large Flash Swap
    Identify large swap values based on a predetermined threshold

Price Impact
    Identify significant price changes based on swap data for a specified list of pools

Change in Liquidity
    Identify significant liquidity changes for a specified list of pools

Loan for Governance Event
    Identify when large loans are used to fund votes on governance proposal

Address Watch
    Monitor transactions involving addresses from an editable watchlist.

Stable Coin Asset Price Tracking
    Tracks price of all assets in the basket alerts on loss of value above a settable threshold.

Account Balance
    Tracks when an account cannot perform action because the balance has dropped

Failed Transaction Monitor
    Monitors failed or pending transactions greater than threshold for Administrative accounts

Failed Swaps
    Monitors failed Swaps greater than threshold

High Transaction Amount
    Monitors any transaction whose value exceeds a threshold.

### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._

We will be using the Forta SDK. We have been working very closely with the Forta team by becoming Forta development partners which allows us to be notified immediately of any change to the SDK as well as provide feedback to Forta for SDK improvements.

### Team description
_Who are your team members, what is your background and what you built before._

Arbitrary Execution (AE) is a blockchain security company made up of security researchers that provides services for smart contract auditing, design consulting, software research and development, and training. AE's security researchers have extensive experience in finding exploitable vulnerabilites both on and off the blockchain.

AE has been actively involved in the pre-launch beta testing of the Forta network and has extensive experience developing Forta agents like the agents being proposed for this grant for Perp.Fi, UniSwap, UMA and Aave.

Below are the Forta Agent developers at AE that would work on this project.

Alexis Williams graduated from Purdue University in 2019 with a Bachelor’s in Computer Science and has since been working professionally as a software engineer and security researcher. Alexis previously worked at ManTech and Novetta providing vulnerability research and software engineering on embedded platforms and leading research on emerging operating systems. She brings a blend of traditional software and security knowledge to emerging blockchain technologies and is excited to make an impact.

Philip Gillett has experience in security research, software development, signal processing, and acoustics research. He conducted wind tunnel, water tunnel, and scale model hydroacoustic research for the US Navy for six years before transitioning to computer security research in 2016. He worked as a principal investigator on using commercial-off-the-shelf devices to perform geolocation of wireless transmitters and as a technical lead developing software to live-update wireless firmwares on commercially prevalent devices. Philip has experience with the scientific computing languages MATLAB and LabView, with the general-purpose programming languages Python, JavaScript, Golang, C, ARM assembly, and with the smart contract language Solidity. Philip has a BS and a PhD in Mechanical Engineering from Virginia Tech and is a licensed PE in Virginia. 

Jasper Clark has worked in the computer security realm for 15 years supporting award winning, multi-million dollar government contracts. Over the years he has attended numerous security 

### Others	 
Anything else you want to share with us

Relevant Links:

Arbitrary Execution
Home: https://www.arbitraryexecution.com/
Github: https://github.com/arbitraryexecution
Twitter: https://twitter.com/Arbitrary_Exec
Blog: https://medium.com/@arbitrary_execution

Forta
Home: https://forta.org/
Github: https://github.com/forta-protocol
Documentation: https://docs.forta.network/en/latest/
Twitter: https://twitter.com/fortaprotocol
Discord: https://discord.com/invite/KACdTEutQq

