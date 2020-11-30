# Proposal Guideline 

## Project Overview

### Project name
Prediction of prediction markets performance.
### Team members 
Victor Porton
### What project are you building 
Allow users to choose between several competing prediction markets predicting future voting about choice of predictions markets. Finance creation of prediction oracles from future funds.
### Why did you decide to build it 
It is useful to make the Internet invest into predicting future performance and influence of for example free software authors, scientists, inventors, with the purpose to reward them now for the future effect. Make fundamental science and free software a profitable commerce. Get rid of patents and proprietary licenses by making free ones more profitable.
### How long will it take 
A few weeks.
### How much funding are you requesting  
Please decide a sum in favor of me.
### How did you hear about the GECO
https://gitcoin.co/issue/gnosis/GECO/75/100023743

## Your Proposal 
### Project description
The following is a mathematical model (applicable to science financing but not only) possible to implement in blockchain for stimulating market to implement the author and publisher scoring oracles.

1. Using a special smart contract anybody can claim his account as a science author for purposes of his “salary” accounting.
2. Using a special smart contract anybody can claim his account as a science publisher.
3. Anybody could create (if he has enough money to implement this) an oracle mapping for example scientist’s Ethereum address to the scientist’s score (such as based on the number of direct and indirect citations and on how free the manuscript license is) (accordingly this oracle) and optionally to the publisher(s).
4. Create two prediction markets:
    1. the score of each oracle
    2. the score of each scientist and each publisher by each oracle (so NxM where N is the number of scientists and M is the number of oracles outcomes)
5. Allow anybody to deposit ETH (or a token) to be exchanged for the collateral (after 100+ years, see below). It can be made with something like Uniswap.
6. After 100 years each oracle owner is expected to write the “score” (presumably based on citations counts and licensing/pricing policies) for each scientist (with nonzero results) into the blockchain. He is also expected to score publishers. (A probably simplest way to score publishers is to add scores for all articles for which it is is considered the primary publisher.)
7. During some additional time period the people (or robots) vote resulting scoring each of these oracles 0..1 (with the sum 1) based on how they perceive the “correctness” or “fairness” of its scientists’ scores. The voting results are the outcomes of the oracles list predictions.
8. Each oracle receives the collateral proportional to its score.
9. Each scientist receives the collateral proportional to the sum of the products of his score in an oracle to the score of the oracle. (To be retrieved from each oracle funds separately, because potentially there may be many oracles.)
10. Each publisher receives the collateral proportional to its score.

So, we have the prediction markets for scientists, publishers, and oracles, they receive some reward now (not after 100 years).
How to split the collateral into three parts between scientists, publishers, and oracles? It could be done by voting after 100 years with voting results taking the arithmetic averages from each voter. Or we can start voting now and keep it running for 100 years.
We could also pay to reviewers but that’s not possible to do fairly as they are anonymous.
### Features
Solidity, JavaScript tests.
### Team description
Victor Porton (`vporton` at GitCoin) - a frequent and respected GitCoin contributor.
### Timeline, Milestones and Deliverables

**Phase I**
Whitepaper.

**Deliverables**
Whitepaper.

**Time and Price Estimate**
6 days.

**Phase II**
Smart contracts.

**Deliverables**
Compilable smart contracts.

**Time and Price Estimate**
10 days.

**Phase III**

**Deliverables**
Testing smart contracts.

**Time and Price Estimate**
3 days.

### Others
[More information](https://reward.portonvictor.org/predict-prediction-markets-or-hire-google-to-account-salaries-for-scientists-and-free-software-developers/)

Need first finish:
* https://github.com/gnosis/GECO/pull/79
* https://github.com/gnosis/GECO/pull/81