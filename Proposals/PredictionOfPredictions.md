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
$3000 because the project is complex.
### How did you hear about the GECO
https://gitcoin.co/issue/gnosis/GECO/75/100023743

## Your Proposal 
### Project description
* [Visual diagram to grasp it better.](assets/PredictionOfPredictions-diagram.pdf) (PDF)
* [Short presentation slides.](assets/PredictionOfPredictions-slides.pdf) (PDF)

The following is a mathematical model (applicable to science financing but not only) possible to implement in blockchain for stimulating market to implement the author and publisher scoring oracles.

1. Using a special smart contract (similar to my [ConditionalTokensMany.sol](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/contracts/ConditionalTokensMany.sol)) anybody can claim his account (just call a special contract method with his Ethereum address and probably some identity like first/last name) as a science author for purposes of his “salary” accounting. Simply, due to technical limitations of ERC-1155, a user needs to be explicitly registered before he can receive tokens.
2. Using a special smart contract (ditto) anybody can claim his account as a science publisher.
3. Anybody could create (if he has enough money to implement this) an oracle (a possibly off-chain software that may write data to the chain using a specially provided method) mapping for example scientist’s Ethereum address to the scientist’s score (such as based on the number of direct and indirect citations and on how free the manuscript license is) (accordingly this oracle) and optionally to the publisher(s). That is oracle is a software that stores into the chain scientists "score" (a number which his salary is proportional to, calculated accordingly the oracle's creator's sense of fairness). With an oracle is also associated an address that will hold collateral funds for this oracle (after 100 years), to be further distributed among scientists.
4. Create two prediction markets:
    1. the score of each oracle
    2. the score of each scientist and each publisher by each oracle (so NxM where N is the number of scientists and M is the number of oracles outcomes)
5. Allow anybody to deposit ETH (or a token) to be exchanged for the collateral (after 100+ years, see below). It can be made with something like Uniswap.
6. After 100 years each oracle owner is expected to write the “score” (presumably based on citations counts and licensing/pricing policies) for each scientist (with nonzero results) into the blockchain. He is also expected to score publishers. (A probably simplest way to score publishers is to add scores for all articles for which it is is considered the primary publisher.)
7. During some additional time period the people (or robots) vote resulting scoring each of these oracles 0..1 (with the sum 1) based on how they perceive the “correctness” or “fairness” of its scientists’ scores (for our purposes we define correctness/fairness of an oracle as the quantity of votes an oracle will receive). The voting results are the outcomes of the oracles list predictions.
8. Each oracle receives the collateral proportional to its score.
9. Each oracle's collateral holder receives 
9. Each conditional token holder can receive (after 100 years, for any oracle) the collateral proportional to the product of his score in an oracle to the score (voting result) of the oracle using two consequtive transfers: 1. to oracle's collateral holder from the |prediction of predictions" contract; 2. from that collateral holder to the requestor of funds. (To be retrieved from each oracle funds separately, because potentially there may be many oracles.)
10. Each publisher receives the collateral proportional to its score.

We have thus a prediction market that will run for about 100 years.
As I explain in [this note](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/docs/future-money.rst), this kind of prediction markets is similar to transferring money from the future.
So, we have the prediction markets for scientists, publishers, and oracles, they receive some reward now (not after 100 years).
How to split the collateral into three parts between scientists, publishers, and oracles? It could be done by voting after 100 years with voting results taking the arithmetic averages from each voter. Or we can start voting now and keep it running for 100 years.
We could also pay to reviewers but that’s not possible to do fairly as they are anonymous.

The icentives to put a collateral into this market are:

- goodwill to help the scientists, etc.
- the donor will receive more voting rights.

The market resolves only after 100 years, but as we know conditional tokens have value even before the market resolves. It incentivizes to trade the tokens meantime.

Note that I expect both individuals, corporations, and governments to donate, too. Because 100 years is apparently after the Second Come of Christ, it's likely that both individuals and corporations will be made much more generous than now. Also appearance of a world goverment that could use my software to support scientists around all the world seems likely during 100 years independently on your religious views.

The above needs to be modified (as will be described in the planned whitepaper) to pay salaries to scientist not one time (because this would be too dangerous to allow people to spend all their lifetime salary in one transaction) but proportional to the time since registration. This requires BrightID integration to check if a scientist is still alive.

#### The current status and technical details

I have developed [ConditionalTokensMany.sol smart contract](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/contracts/ConditionalTokensMany.sol) (development finished but not enough tested yet).

This contract needs to be modified to include BrightID integration and based on this payments proportional to the time since registration rather than one-time payments.

BrightID has "supervisor" feature, that need to be integrated into the contract for greater fraud resistance. I am going to use my own BrightID node (please also provide funding for a server to run this node) as the oracle (unrelated with "scoring" oracles described above) for supervising BrightID. The supervising oracle needs to be an upgradeable smart contract, because otherwise it would remain centralized. Upgrading the BrightID supervising oracle needs to be done by voting. The voting contract needs also be upgradeable (by itself, the voting contract). Our initial voting contract is going to be quadratic with BrightID anti-sybil and vote weight proportional to the square root of the amount of WETH (I've choosen this ERC-20 token arbitrarily) donated to the system by a given voter.

Also need to add restoration of lost scientists' accounts via BrightID.

BrightID integration is the most complex part of the system.

Need also to consider replacing BrightID by Ceramic identity. (I still haven't studied the features of Ceramic, so I will revise this document after I study Ceramic.)

I am going to work on this project after I finish [ConditionalTokensMany.sol smart contract](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/contracts/ConditionalTokensMany.sol):

- need to test it thoroughly
- need to add virtual functions to be able to use BrightID and salary withdrawal amounts proportional to the time passed rather than one-time.

The contracts to be produced:

- the "prediction of predictions" conditional tokens contract (modified [this contract](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/contracts/ConditionalTokensMany.sol)) that also accepts donations
- the prediction markets contract that can receive the collateral assigned to a given oracle proportionally to the voting results for this oracle and then distribute to the traders (conditional token holders) accodingly to their score by this oracle (slightly modified [this contract](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/contracts/ConditionalTokensMany.sol) will suffice)
- the upgradeable voting contract
- the upgradeable BrightID supervisor contract

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
9 days, $1000.

**Phase II**
Smart contracts.

**Deliverables**
Compilable smart contracts.

**Time and Price Estimate**
12 days, $1000.

**Phase III**

**Deliverables**
Testing smart contracts.

**Time and Price Estimate**
5-6 days, $1000.

### Others
[More information](https://reward.portonvictor.org/predict-prediction-markets-or-hire-google-to-account-salaries-for-scientists-and-free-software-developers/)

Need first finish:
* https://github.com/gnosis/GECO/pull/81
