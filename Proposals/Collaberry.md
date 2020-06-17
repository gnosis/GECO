# Collabery Safe App (3rd keys)

replace Upwork escrow with a market of 3rd keys

## Overview

Collabery aims to replace the Upwork escrow function with a 2-out-of-3 Safe and a market of mediators (3rd keys). As a result,  the fair price of this service and the growth of its quality.
The mediator withholds a commission for his services in the form of % of the job cost.
The platform holds a commission in the form of % of the mediator's commission.
The commission of the platform can be used to maintain a minimum infrastructure and to create the necessary incentives.

## Flow

The mediator creates a 2-out-of-3 Safe with the addresses of the freelancer and the customer.
The mediator creates a job, including the description, cost, and address of the managing safe.
Freelancer does the work and sends the result to the mediator and the customer
The mediator performs the necessary mediation between the freelancer and the customer, the result of which should be a mutually beneficial agreement.
The mediator generates a final transaction, including payment to the freelancer, refund to the customer, mediator commission, platform commission, and updating the status of the job.

## Interface

should allow registering a mediator,
filter mediators,
create a job, 
make a deposit, 
generate a final transaction,
display the latest activity on the platform.

## Architecture

Mediator has an address, description, and commission %.
Managing Safe is 2-ot-of-3 Safe with a mediator, freelancer, and customer addresses.
Job has a Managing Safe, description, cost, and status.
A smart contract of the platform stores a mapping of Mediators and an array of Jobs.
Mediator, freelancer, and customer are coordinated through the Telegram bot.


## Possible improvements

Extend the final transaction with 2 feedbacks from the freelancer and the customer.

Add the option to leave feedback to the mediator from the freelancer and the customer.

Use part of the platform commission to create important incentives using referral bonus and dividends.

**Referral program**

Pay bonuses to the inviters and inviters of inviters to create a network effect.

**Dividends**

In exchange for the platform commission, the user will receive platform tokens, which will be used to dividends payout.

Referral program and dividends can be implemented via Telegram bot.

## Team members

Max Pogorelov - master of computer science, full-stack developer with an experience of building production-ready smart contracts, founder of Tipsomat (tipsomat.com), and also experienced Upwork user who successfully used 2-out-of-3 Gnosis wallets few times to exclude voracious intermediary.

## Motivation

As an experienced Upwork user, I can say that to maximize profits, Upwork is ready to sacrifice user convenience and privacy. I would like to create a product that will provide a better alternative where Upwork fails, put users interests first, creates an incentive to invite more users and benefit from the product success. The product should not limit but expand opportunities, recommend the best tools and practices, and finally bring more users to crypto.
