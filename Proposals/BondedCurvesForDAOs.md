# GECO app

## **Project Overview**

---

### **Project name**

Bonded Curves for DAOs

### **Team members**
Jordan Ellis <https://github.com/dOrgJelli>  
Asgier Sognefest <https://github.com/sogasg>  
Seth Fabius <https://github.com/sethfork>  
Ori Shimony <https://github.com/oshimony>  

Advisor: Matan Field (DAOstack)  

### **What project are you building**

We are giving DAOstack DAOs like dxDAO the ability to launch and interact with token bonding curves. A DAO will be able to opt-in to this functionality by registering the BondedCurve scheme to its governance controller. Once registered, the DAO can 1) launch a new continuous token with one of the supported reference implementations, 2) modify the bonded curve's parameters, and 3) buy and sell from the curve.  

All of the DAO's interactions with the curve are performed through proposals. We will build an integration for Alchemy Earth (DAOstack's U.I.) that allows the DAO's reputation holders to submit proposals that execute the functionality described above.  

It will also be possible for the DAO (through other schemes) to assign additional functionality/utility to the token. For example, a balance of the token could be required to call certain functions in a dApp owned by the DAO.  

### **Why did you decide to build it**

Most existing use-cases for token bonding curves do not address the governance of the funds that are generated through the activity of speculators. At the same time, most existing DAOs lack sound valuation models and, largely as a result, sustainable sources of funding.  

Creating a bridge between token bonding curves and the DAOstack governance framework will allow new DAOs like dxDAO, Genesis Alpha, polkaDAO and others to experiment with new models for DAO valuation. This would create accountable mechanisms for speculators to invest in promising DAOs. Because the DAO's governance is fully transparent, speculators can easily track fund usage and remove or add support on that basis.  

For instance, dxDAO could launch a continuous token on a bonding curve that gives token-holders a self-enforcing claim on future DutchX fees. We would expect the price on such a curve to reflect the dxDAO's [Present Value of Future Cash Flows](https://www.investopedia.com/articles/fundamental-analysis/11/present-value-free-cash-flow.asp). Such a scheme could bootstrap the dxDAO's treasury, allowing it to fund the development of DutchX and other dApps ahead of significant revenues from dApp fees.  

### **How long will it take**

5 months

### **How much funding are you requesting**

$50,000

### **How did you hear about the GECO**

Word of mouth

## **Your Proposal**

---

### **Project description**

Token bonding curves come in many different shapes and sizes. Configurations can vary across various factors including:  

- C*urve*: linear, exponential, polynomial, square root, sigmoid  
- *Reserve Currency*: ether, particular erc-20's  
- *Spread:* difference between buy & sell curves that goes to the DAO  
- *Time Locks*: prevent pump & dumps by restricting sells for a certain period after purchase or until tiered thresholds are met  
- *Front-Running Guards*: batching, gas price caps  
- *Additional Functions*: burn, beneficiary buyback, etc.  
- *Mutability*: can curve parameters be changed after launch?  

Bonding curves are also being implemented for a variety of use-cases:  

- *Automated Market Makers* enable seamless, real-time token swaps that eliminate the need to match buyers and sellers (e.g. DutchX, Bancor)  
- *TCR's & Curation Markets* allow communities to curate lists and signal support for different memes or social causes (e.g. Ocean Protocol, Zap)  
- *Continuous Organizations* let organizations raise funds on an ongoing basis while keeping them accountable to contributors  

Each use-case requires a designer to configure the curve according to particular goals, user classes and attack vectors.  

We believe that DAOs like dxDAO are best-positioned to realize such use-cases in the pursuit of their stakeholders' goals. For this reason, we want to build the tooling to make it easy for DAOs to launch, manage and interact with their own bonding curves.  

### **Features**

This functionality will be built on top of and integrated with DAOstack's existing software stack. Our implementation will take the form of:  

**On-Chain Functionality**

- DAOstack Scheme:  
    - Buy (Mint) & Sell (Burn) Tokens  
    - Create Bonding Curve Market  
    - Modify Bonding Curve Parameters  

**Application Functionality**

- Alchemy Earth Integration:  
    - Create Proposals  
        - Proposal will trigger a vote for initiating a bonding curve with the specified parameters  
        - The user will be able to specify parameters like curve, reserve token, spread, time locks etc., when creating the proposal  
        - Proposed bonding curve and associated parameters will be displayed to the DAO's reputation holders in an intuitive way  
    - View DAO's Token Holdings  
    - View DAO's Curve  
        - Buy / Sell History  
        - Circulating Token Supply  
        - Market Reserve Balance  

### **Team description**

We are members of [dOrg](https://github.com/dOrgTech), a freelancer cooperative building open-source DAO tooling.

Matan from DAOstack will also be advising on scientific, economic and architectural design decisions.  

### **Timeline, Milestones and Deliverables**

**Phase I: On-Chain Contracts**

**Deliverables:**

1. DAOstack Scheme

**Time and Price Estimate:** $25,000 for 2.5 months

**Phase II: Application Integration**

**Deliverables:**

1. Alchemy Earth Integration

**Time and Price Estimate:** $25,000 for 2.5 months

### **Others**

You can find a summary and links to our current projects [here](https://github.com/dOrgTech/vision/blob/master/README.md).