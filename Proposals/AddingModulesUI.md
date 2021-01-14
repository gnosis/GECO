# Add an UI for adding a module
## Project Overview

### Project name
> UI for adding a module
### Team members 
> Victor Porton <porton@narod.ru>
### What project are you building 
> An UI for easily adding a module to the wallet
### Why did you decide to build it 
> I want to make modules work in practice.
### How long will it take 
> 10 days
### How much funding are you requesting  
> $5000 in stETH or ETH
### How did you hear about the GECO
> I don't remember.

## Your Proposal 
### Project description
Change `Advanced` section of `Settings` to be able to easily add a module.

The proposal of this grant is limited to adding modules that can be initialized by a call to a method without arguments. (Doing otherwise would require to be able to query something (like EtherScan) for the API specs, this is outside of the scope of this proposal.) It will be presented a dialog widget asking for (optional) the name of the function to be called with the default to be `setup` and the address of the module. There will be also text advising to use APPS tab to install "standard" modules (that I am going to add in other grants). The UI should display a message and if anticipated do other relevant UI changes.

Writing a phone app is outside of the scope of this proposal.

I want to do this stuff because:

* I am a Gnosis Safe user and want to use modules myself.
* I am a creating the [https://github.com/gnosis/safe-modules/pull/23](`Bequest` module) that I also use in my other project, and I want to be able to make its UI, too, so this series of proposals.

The goal is to make modules well supported in UI.

You should fund me because modules are very important and thus we need a generic UI for them (even if there is no App for a particular module).
### Features
I provide a PR for https://github.com/gnosis/safe-react and possible related repositories as appropriate.

I use React. I use an appropriate (accordingly a further research) dailog UI.
### Team description
Victor Porton <porton@narod.ru> - a regular GitCoin contributor, creator of many smart contracts and several dApps including React ones.
### Timeline, Milestones and Deliverables
**Phase I**
Creating UI.

**Deliverables**
Fully functinal UI.

**Time and Price Estimate**
10 days, $5000.

### Others	 
I apply for several GECO grants at once, so I it is assumed that I do not do them simultaneously.

I do not warrant beautiful UI (it can be made more beautiful later), however I do implement a quality UX.
It is assumed that high beauty of the UI is not a criterion for the payout for this grant.
