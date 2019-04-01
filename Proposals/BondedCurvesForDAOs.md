# GECO app

## **Project Overview**

---

### **Project name**

Bonded Curves for DAOs

### **Team members**

Ori Shimony, Jordan Ellis, Cory Dickson, Asgier Sognefest

### **What project are you building**

We are giving DAOstack DAOs the ability to launch and interact with token bonding curves. A DAO will be able to opt-in to this functionality by registering the BondedCurve scheme to its governance controller. Once registered, the DAO can 1) launch a new bonded curve market maker with one of the supported 3rd party protocols, 2) modify curve parameters, and 3) buy and sell from a curve.

All of the DAO's interactions with the curve are performed through proposals. We will build an integration for Alchemy Earth (DAOstack's U.I.) that allows the DAO's reputation holders to submit proposals that execute the functionality described above.

### **Why did you decide to build it**

Most existing use-cases for token bonding curves do not address the governance of the funds that are generated through the activity of speculators. At the same time, most existing DAOs lack sound valuation models and, largely as a result, sustainable sources of funding.

Creating a bridge between the many token bonding implementations and the DAOstack governance framework will allow new DAOs like dxDAO, Genesis Alpha, polkaDAO and others to experiment with new models for DAO valuation. This would create accountable mechanisms for speculators to invest in promising DAOs. Because the DAO's governance is fully transparent, speculators can easily track fund usage and remove or add support on that basis.

For instance, dxDAO could launch a token bonding curve that gives token-holders a self-enforcing claim on future DutchX fees. We would expect the price on such a curve to reflect the DxDAO's [Present Value of Future Cash Flows](https://www.investopedia.com/articles/fundamental-analysis/11/present-value-free-cash-flow.asp). Such a scheme could bootstrap the dxDAO's treasury, allowing it to fund the development of DutchX and other dApps ahead of significant revenues from dApp fees.

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
    - Buy / Sell Tokens
    - Create Bonding Curve Market
    - Modify Bonding Curve Parameters

**Application Functionality**

- Alchemy Earth Integration:
    - Create Proposals
    - View DAO's Token Holdings
    - View DAO's Curve
        - Token Supply
        - Buy / Sell History
        - Market Reserve Balance

### **Team description**

We are members of [dOrg](https://github.com/dOrgTech), a freelancer cooperative building open-source DAO tooling.

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