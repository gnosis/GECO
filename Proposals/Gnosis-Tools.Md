
# Gnosis Grant Application

## Project Overview

### Project name: Gnosis Tools

### Team members

* Prastut Kumar - [Github](https://github.com/prastut), [Linkedin](https://www.linkedin.com/in/prastut1/)
* Sahil Nanda - [Github](https://github.com/sahilnanda1995), [LinkedIn](https://www.linkedin.com/in/sahil-nanda-8b1b88143/)


### What project are you building 

*Gnosis Tools* is an umbrella platform for tooling support around Gnosis ecosystem. For it's first MVP we plan to ship a unified dashboard with the following features: 
* Information and various statistics around Gnosis Safe. 
* Gnosis Gas Station. 

### Why did you decide to build it 

Gnosis team has shipped a wide range of products ranging from open prediction market applications, decentralized trading protocols, and tools to manage funds and interact with the decentralized web. 

When we read through the decks Gnosis team had created for project ideas [Gnosis Statistics Dashboard](https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description-%20Statistics%20Dashboard.pdf) & [Gnosis Gas Station](https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description%20-%20Gnosis%20Gas%20Station.pdf), we reached an awareness that a tooling platform around Gnosis ecosystem would be valuable to the community, where these ideas can serve as the first round of features the platform will have.

 
In the future, we're hoping to enrich the platform by providing analytics/support to other products in the Gnosis ecosystem. 


### How long will it take 
6 weeks

### How much funding are you requesting  
$10,000 

### How did you hear about the GECO
Word of mouth. 

## Your Proposal 
### Project description


We plan to create a unified dashboard which will provide an interface to solve for the usecases mentioned in [Gnosis Statistics Dashboard](https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description-%20Statistics%20Dashboard.pdf) & [Gnosis Gas Station](https://github.com/gnosis/GECO/blob/master/Project%20Ideas/Project%20description%20-%20Gnosis%20Gas%20Station.pdf) decks. 


### Pre-Proposal Stage

What we did before writing this proposal: 

* Gained [vantage on the data Gnosis API](https://hackmd.io/L_gXqfAeQeGUn5f6P-nYYg?both#API-Links) provides to come up with the UX of the dashboard. 
   
* Iterated through several brainstorming sessions to create [mock-ups](https://www.figma.com/file/4pVf2Lkouxk7ioR9IyBcRm/Gnosis-Safe-Statistics-Dashboard?node-id=153%3A694) for the dashboard. [Protypes in action.](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A695&scaling=min-zoom)


### Features

![](https://i.imgur.com/jL6AMfc.jpg)


#### Overview of the Gnosis Tools Platform: 

Dashboard is currently divided into 2 categories: 
* Safe Statistics: 
    * Overview - offers users vantage over what's happening inside the Gnosis safe from a bird's eye view. 
    * Token Analytics - offers search interface to user users where they can search for the token they want token specific analytics on. 
        * Specific Token Analytics: when user clicks on a specific token, they are shown token specific analytics.  
* Gas Station: 
    * Overview - offers users the option to select the payment token for which they want to see gas prices for + the ability to calculate gas prices in payment token's unit by inputting the gas used by their contract.
    * FAQ's  - for information around how gas prices are being calculated. 


[Protypes in action.](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A695&scaling=min-zoom)

### Tech Specs: 

Development Stack: 
* [React.js](https://reactjs.org/)
* [Ant Design for UI Framework](https://ant.design/)
* [BizCharts for charts](https://github.com/alibaba/BizCharts)

Hosting: since the dashboard can be a pure client side app, we might explore services like [Surge](https://surge.sh/) or [Zeit's Now](https://zeit.co/). 


### Team description


#### Prastut
Currently a partner @ The Vantage Project. Comes from a UX, product management & full stack background.

Relevant data visualization, UI/UX experience: 
* Executed [PolkaViz](http://polkavizproject.surge.sh/) as part of PolkaDAO. PolkaViz aims to kickstart data visualization efforts around the Polkadot ecosystem. Kickstarted and developed 40% of the project + supervised Sahil who executed 60% of the project. (2019)
* Co-founder, Designer, Frontend Developer for [Centify](https://centify.surge.sh/) (2018). Built the entire frontend data visualization stack. 
 * Data Visualization Research Associate at Information Design Lab, IIT Bombay (2017). [Work documentation](https://prastut.github.io/dataviz ).  
        

[Github](https://github.com/prastut), [CV](https://drive.google.com/file/d/15_oS6XtO_DRlITjG6WyTAEavaiSnBsdL/view?usp=sharing), [LinkedIn](https://www.linkedin.com/in/prastut1/). 

#### Sahil: 

Software developer @ The Vantage Project. 

Relevant data visualization experience: 
Executed 2/3rd of the PolkaViz as part of PolkaDAO. 

[Github](https://github.com/sahilnanda1995), [LinkedIn](https://www.linkedin.com/in/sahil-nanda-8b1b88143/). 

 


## Timeline, Milestones and Deliverables


#### Phase 1

Deliverables:
- Finish laying down the foundation for the dashboard.
- [Safe Statistics Overview](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A695&scaling=min-zoom) will be deployed live. 


Time and Price Estimate: 
- Time: 2 weeks
- Price Estimate: $4,000


#### Phase 2

Deliverables:
- Development and deployment of all the components shown in the below links:
    * [Token Analytics - search interface for tokens stored inside Gnosis Safe](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A1426&scaling=min-zoom)
    * [Specific Token Analytics](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A1426&scaling=min-zoom)
    * [Gas Station Overview - display gas prices for different speeds, gas price history, gas price calculator](https://www.figma.com/proto/4pVf2Lkouxk7ioR9IyBcRm/Gnosis---Safe-Statistics-Dashboard?node-id=153%3A931&scaling=min-zoom)

Time and Price Estimate
- Time: 2 weeks
- Price Estimate: $4,000 USD

#### Phase 3

Deliverables: 
- FAQ section for gas price. 
- Installation instructions uploaded to the Github repo of the dashboard. 
- Screencast guiding through the dashboard. 
- Buffer time of 1 week kept for delays.  

Time and Price Estimate
- Time: 2 weeks
- Price Estimate: $2,000 USD


### Reporting
Weekly reports will be submitted in the [#gnosis-gitter](https://gitter.im/gnosis/GECO) channel. The community can keep us accountable by going through each step described in the timeline & double check if these were implemented.

## Remarks
Our team will be working full time on this project. 

Additionally, we would be more than happy to listen and incorporate the communities feedback and make changes (if any) on the mockups of the proposed design. 


## Appendix: 

### API Links: 
 * Number of safes (deployed, not deployed), funds stored(ETH and other supported tokens): https://safe-relay.gnosis.pm/api/v1/stats.
* Funds created over time, number of transactions per day, % of payment tokens used for transactions over time,  Volumes over time: https://safe-relay.gnosis.pm/api/v1/stats/history.
* Tokens Info: https://safe-relay.gnosis.pm/api/v1/tokens/. 
* Payment Tokens: https://safe-relay.gnosis.pm/api/v1/tokens/?gas=true.
* Gas Price Info: https://safe-relay.gnosis.pm/api/v1/gas-station/.
* Gas Price History: https://safe-relay.gnosis.pm/api/v1/gas-station/history.
