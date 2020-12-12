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

1. Using a special smart contract anybody can claim his account (just call a special contract method with his Ethereum address and probably some identity like first/last name) as a science author for purposes of his “salary” accounting. Simply, due to technical limitations of ERC-1155, a user needs to be explicitly registered before he can receive tokens.
2. Likewise, using a special smart contract (ditto) anybody can claim his account as a science publisher.
3. Anybody could create (if he has enough money to implement this) an oracle (a possibly off-chain software that may write data to the chain using a specially provided method) mapping for example scientist’s Ethereum address to the scientist’s score (such as based on the number of direct and indirect citations and on how free the manuscript license is) (accordingly this oracle) and optionally to the publisher(s). That is oracle is a software that stores into the chain scientists "score" (a number which his salary is proportional to, calculated accordingly the oracle's creator's sense of fairness). With an oracle is also associated an address that will hold collateral funds for this oracle (after 100 years), to be further distributed among scientists.
4. Create two prediction markets:
    1. the score of each oracle
    2. the score of each scientist and each publisher by each oracle (so NxM where N is the number of scientists and M is the number of oracles outcomes)
5. Mint to each scientist his own conditional token proportional to time passed since his registration. This will be his salary.
6. Allow anybody to deposit a token to be exchanged for the collateral (after 100+ years, see below).
7. After 100 years each oracle owner is expected to write the “score” (presumably based on citations counts and licensing/pricing policies) his conditional token for each scientist (with nonzero results) into the blockchain. He is also expected to score publishers. (A probably simplest way to score publishers is to add scores for all articles for which it is is considered the primary publisher.)
8. During some additional time period the people (or robots) vote resulting scoring each of these oracles 0..1 (with the sum 1) based on how they perceive the “correctness” or “fairness” of its scientists’ scores (for our purposes we define correctness/fairness of an oracle as the quantity of votes an oracle will receive). The voting results are the outcomes of the oracles list predictions.
9. Each oracle receives the collateral proportional to its score.
10. Each conditional token holder can receive (after 100 years, for any oracle) the collateral proportional to the product of his score in an oracle to the score (voting result) of the oracle using two consequtive transfers: 1. to oracle's collateral holder from the "prediction of predictions" contract; 2. from that collateral holder to the requestor of funds. (To be retrieved from each oracle funds separately, because potentially there may be many oracles.)

We have thus a prediction market that will run for about 100 years.
As I explain in [this note](https://github.com/vporton/conditional-tokens-contracts/blob/shared-sets/docs/future-money.rst), this kind of prediction markets is similar to transferring money from the future.
So, we have the prediction markets for scientists, publishers, and oracles, they receive some reward now (not after 100 years).
How to split the collateral into three parts between scientists+publishers and oracles? It could be done by voting after 100 years with voting results taking the arithmetic averages from each voter. Or we can start voting now and keep it running for 100 years.
We could also pay to reviewers but that’s not possible to do fairly as they are anonymous.

The incentives to put a collateral into this market are:

- goodwill to help the scientists, etc.
- the donor will receive more voting rights.

The market resolves only after 100 years, but as we know conditional tokens have value even before the market resolves. It incentivizes to trade the tokens meantime.

Note that I expect both individuals, corporations, and governments to donate, too. Because 100 years is apparently after the Second Come of Christ, it's likely that both individuals and corporations will be made much more generous than now. Also appearance of a world goverment that could use my software to support scientists around all the world seems likely during 100 years independently on your religious views.

#### The current status and technical details

I have developed [BidOnAddresses.sol](https://github.com/vporton/conditional-tokens-contracts/blob/bid-addresses/contracts/BidOnAddresses.sol) (development finished but not enough tested yet).

This contract needs to be modified to be appropriate for this proposal:
- Make allocation of conditional tokens proportional to the time since registration rather than one-time as now.
- Allow to restore lost accounts (by a smart contact upgradeable by voting) of scientists, because they otherwise be legible to losing their lifetime salaries.
- So, add voting and ability to upgrade the voting contract itself by voting.
    - Add a nontransferrable voting token.
        - Proportional to donated WETH token (calculation of the amount of voting token should be upgradeable).
        - Myself receive (as the first estimation) $140000 in non-transferrable voting rights to keep the system under my control until enough big players enter.
    - For start voting we can use DAOstack.

A future upgrade of the voting contract is expected to use a DAOstack DAO.

The contracts to be produced:

- the "prediction of predictions" conditional tokens contract (modified [BidOnAddresses.sol](https://github.com/vporton/conditional-tokens-contracts/blob/bid-addresses/contracts/BidOnAddresses.sol)) that also accepts donations
- the prediction markets contract that can receive the collateral assigned to a given oracle proportionally to the voting results for this oracle and then distribute to the traders (conditional token holders) accodingly to their score by this oracle (slightly modified [BidOnAddresses.sol](https://github.com/vporton/conditional-tokens-contracts/blob/bid-addresses/contracts/BidOnAddresses.sol) will suffice)
- the upgradeable voting contract

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
9 days, $750.

**Phase II**
Smart contracts.

**Deliverables**
Compilable smart contracts.

**Time and Price Estimate**
12 days, $750.

**Phase III**

**Deliverables**
Testing smart contracts.

**Time and Price Estimate**
5-6 days, $750.

**Phase IV**

**Deliverables**
A dapp.

**Time and Price Estimate**
5-6 days, $750.

### Others
[More information](https://reward.portonvictor.org/predict-prediction-markets-or-hire-google-to-account-salaries-for-scientists-and-free-software-developers/)

Need first finish:
* https://github.com/gnosis/GECO/pull/81
