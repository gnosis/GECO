# Jiffy Proposal 

## Abstract

Ethereum allows developers to create applications without worrying about servers, frontend, security of data and a plethora of other stuff web2.0 applications have to worry about. Its a great feeling to deploy the contract on a testnet and just share the contract address to possible users. Interacting with contracts deployed is tough without a dedicated front-end even for experienced technocrats, you have to get the abi, contract address,make sure he/she has ether, know the inputs and expected outputs to make sure you are doing it right. A user runs out of patience and/or motivation to try out your contract if he has to go through so much hassle. We want to encourage on boarding of new users so that they can interact with contracts in a **jiffy** without worrying about the overhead stuff. We want to make trying out contracts as straight-forward as possible for new users as well as existing devs.


### Features

    - Creation of markdown labels/widgets/QR(anything behind which we can hide a URI :)) which can be attached to readme files of github repo, users can just click that to send a single or multiple transactions for a required functionality.For Example: approve and transferForm can be done with a single label. Interesting thing to note is these labels can also become `testing` or `autoDeployment` tools with no changes whatsoever.
    
    - Allowing meta transactions ie users can interact with the contract with erc20 tokens or with no ether/erc20 tokens. We plan to allow the contract creators to `seed` their contract with some ether/tokens using which initial users can interact with contracts with no ether or token.
    
    - Every contract will have a unique URI which can be shared everywhere just like domain name, users could visit the URL and interact with the whole contract ,we allow the contract owner to pin frequently used dapps at the top for better usability.
    
    - Allowing users to watch a specific types of transactions using ethereum events. For example a user may like to get an email when he gets some tokens , when someone withdraws from his multisig, when someone interacts with one of his contracts and a 1000 other cases. Users will be able to watch these events easily and be at ease.
    
    - View dapps by traffic , recently created and multiple other categories.
    
    - Allow users to bunch together different labels created by others. For example someone created a label for "Approve and transferFrom" , you could add "StakeFor" to it and display it on your readme as "Staking" for your contract implementing EIP 900.
    
    - Matching contract to nearest interface. For example we could show contracts that match ERC-20 interface by percentage while user is interacting with it.So you would know that you are interacting with a contract which is 80% ERC20 .
    
    - `Create PWA for your dapp` using which users after being redirected to a particular contract can pin it to their homescreen by creating a PWA for using later. 
    
UI/UX , usability being the primary motivation we aim to bring new users onboard as quickly as possible without knowing anything about blockchain. This could also help in first experimenting with new contracts/dapps without building a front end and then when dapp gains enough traction you can build a custom UI/UX
   
### Deliverables

We have several things in the roadmap to make this happen:

    1. Creation of Mockups, Database models. 
    2. Contract Registration.
    3. Label Registration.
    4. AUTH using ethereum signatures.
    5. Meta Transaction support. 
    6. Event Watchers.
    7. Contract Interface Matching. 
    8. Create PWA for dapp.
    9. Sort dapp by various categories.
    
  
##### Tech Stack 

We will be using React+Typescript on the frontend and golang on the backend with mongodb as the database


## Grant size

Funding: 60k-80k USD worth ETH,delivered in chunks paid out before/after achieving deliverables

## Integrations

We dont want to reinvent the wheel we want to build a car hence we encourage use of existing solutions to build up synergy.
1. Dappratus(https://github.com/austintgriffith/dapparatus)
2. Dagger(https://matic.network/dagger/)
3. Remix 
4. EthFiddle

### Team
 
#### Vaibhav Chellani - Project Lead, Blockchain and Backend Developer
Commitment: Part time 
Links: github(https://github.com/vaibhavchellani)

#### Shubham Singh - Full Stack Developer
Commitment: Full time 
Links: github(https://github.com/imshubhamsingh)

#### Kautuk Kundan - Front End Developer
Commitment: Full time
Links: github(https://github.com/kautukkundan)

PS: We have completed grant projects for other projects like Zilliqa successfully:  https://github.com/merkaliser/scilla-vanilla

### BurnRate 
5 devs : 2 Full time, 1 Part time
3 - 4 month job 
$20k USD per month 

## Development timeline

The development timeline will be the following one in regards to each deliverable:

1. First Month  -  Deliverable 1,2,3,4
2. Second Month -  Deliverables 5,8,9
3. Third Month  -  Deliverables 6,7
4. Fouth Month  -  Testing and Refactoring 

## Category 

We would most probably lie on the `dapp usability` side . We will allow users to interact with multiple contracts without a custom frontend thus lowering the barrier to create a proper usable product , developers just have to write contracts now!  
