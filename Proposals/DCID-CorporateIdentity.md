# DCID - Decentralized Corporate Identity
_Decentralized Corporate Identity powered by Gnosis contracts_

## Project Overview

### Project name

DCID (Decentralized Corporate Identity)

### Team members 

* Carlos Bruguera (cbruguera@gmail.com)
* Ben Gervais (ben@grvs.io)
* Edmund Lowell (edmund@selfkey.org)

### What are we building?

_Decentralized Corporate Identity_ (or _DCID_ for short) is a project that aims to provide 
Decentralized Identity that's suited for practical corporate use. Powered by Gnosis smart contract 
infrastructure, it allows companies not only to manage funds in a trustless and secure manner via 
Gnosis Safe, but also control the identity aspects of the company. The following are the basic 
*building blocks* of DCID:

* Multisig control of a [Decentralized Identifier](https://w3c-ccg.github.io/did-primer/)
* Issuance and verification of public and private cryptographic credentials
* Extensibility and interoperability with other DID-based identity platforms

We refer to these features as "building blocks" because they allow for a vast spectrum of 
possibilities to be built on top of the identity layer. 

### Why build this?

The specification of [DIDs](https://w3c-ccg.github.io/did-primer/) is a joint effort led by many 
different groups and companies that is gaining significant traction in the last few years as a 
viable solution to _Decentralized Identity_. Thanks to the specs provided by W3C Working Groups and 
the active work of the [Decentralized Identity Foundation](https://identity.foundation/), 
DIDs are likely to become a standard for how individuals and groups control their digitial identity 
in a self-sovereign manner. 

There is no doubt that this important breakthrough is well suited not only for individuals but also 
companies can benefit significantly from a platform that allows to manage their identity. Gnosis 
already provides a fundamental component for digital corporate management: _Gnosis Multisig Safe_. 
We intend to build a layer that allows Gnosis Safe users (corporate and individual) to join the 
decentralized identity ecosystem, extending the existing Safe functionality and opening the doors 
for further development of Gnosis Safe features around digital identity.

### Estimated time

16 weeks

### Funding requested

$ 48,000

## Proposal 

### Project description

The project development consists of the following components:

* A DID ledger smart contract for storing resolvable DIDs and URL endpoints
* Verifiable Credentials smart contracts and libraries
* Universal DID Resolver module ready to be used with SelfKey DID, easily extensible to other DID 
methods.

All smart contracts and libraries will be tested integrating with Gnosis Safe Multisig (React). 
Integration code and tests will be provided as part of the deliverables.

### Features

The project will be developed on top of existing Gnosis Safe functionality on Ethereum, following 
the [DID](https://www.w3.org/TR/did-core/) and [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/) 
generic specs as defined by the corresponding W3C working groups to ensure the interoperability 
among different identity platforms. 

The following is a high level description of this project's features:

#### DIDs and DID ledger

Borrowing the definition from a [W3C community group page](https://w3c-ccg.github.io/did-primer/): 
_“A Decentralized Identifier (DID) is a new type of identifier that is globally unique, resolvable 
with high availability, and cryptographically verifiable. DIDs are typically associated with 
cryptographic material, such as public keys, and service endpoints, for establishing secure 
communication channels. DIDs are useful for any application that benefits from self-administered, 
cryptographically verifiable identifiers such as personal identifiers, organizational identifiers, 
and identifiers for Internet of Things scenarios.”_

We're implementing a _DID ledger_ smart contract that acts as a simple registry for identifiers that 
can be used by on-chain or off-chain resolvers. A DID ledger is not meant to store any sensitive 
information, but should allow retrieving relevant data for authentication and URL endpoints.

Having this identifier layer on top of existing Ethereum addresses allows users to migrate to 
different controllers while keeping their identifier. For example, an identity owner might have a 
DID controlled by a regular account address and then decides to upgrade to a Gnosis Safe while 
keeping their identity along with all associated credentials, later on this identity owner could 
switch to a different multi-sig solution to control their identifier.

#### DID Resolver

A _DID resolver_ javascript library will be implemented that constructs a DID document 
following the [W3C generic specs](https://www.w3.org/TR/did-core/) standard. A resolver's job is to 
"translate" a DID into the public data that corresponds to that identifier (service URL endpoints, 
cryptographic material, etc). In order to remain interoperable with other DID systems, we'll be 
integrating with DIF's [Universal Resolver](https://github.com/decentralized-identity/universal-resolver/), 
allowing Gnosis Safe users to manage or interact with identities from different identity networks.

##### Gnosis-specific resolution method

At SelfKey, we plan to use Gnosis Safe as a fundamental piece of our identity management solutions,
therefore, although DIDs should be generic enough to be controlled by personal Ethereum 
accounts or other proxy contract implementations, our DID resolver will be tailored for using with 
Gnosis Safe, being able to resolve public data stored on Safe contracts through custom modules, 
represent control delegation relationships for complex authentication flows, etc.

#### Verifiable Credentials

One of the main strengths of decentralized identity is to allow identity owners to issue and hold 
"claims" about themselves, other identities or about anything that can be referenced. A set of 
claims made by a given entity can be referred to as a _verifiable credential_ (i.e. authorship can 
be cryptographically verifiable). Depending on the use case and context, credentials may expire or 
be revoked, as they could define complex actionable semantics.

Credentials are meant to disclose only the necessary information for relying parties to verify, 
however, in order to be "time-stampable" and verifiable on-chain, they are anchored to a 
_credential registry_ smart contract. For example, a trusted identity in a given system issues a 
credential stating that the individual controlling a certain _DID_ passed some KYC process, yet 
without disclosing any personal data. Multiple levels of "selective disclosure" can be applied to 
credentials depending on the case.

##### Gnosis-specific credential modules

Turning Gnosis Safe proxies into _identities_ on the blockchain means they should be able to hold
and issue credentials publicly. To this end, we will be implementing Gnosis modules that act as
_credential registries_ allowing smart contracts or off-chain clients to verify public claims associated
with Gnosis Safe proxies. 

Our main goal is to turn Gnosis Safe into more than just a collaborative management of assets, or 
more precisely to _include_ identity material as a different type of asset that can be managed and 
verified by Gnosis Safe owners.

### Team description

We are team members at _SelfKey_, which is a project aiming to build a marketplace for financial 
services while easing up the KYC and identity verification processes for customers and service 
providers. 

There's a lot of room for Gnosis technology in our own development and we have many exciting ideas 
to implement around Gnosis contracts in the context of digital corporate management. The following 
describes each team member and why we are qualified to build this project.

**Edmund Lowell** is an regtech and legal tech entrepreneur innovating at the crossroads of finance, 
technology and law. He has built a number of fintech apps that compare jurisdictional requirements 
for companies (for instance incorporations.io) that will be directly relevant to the DCId project. 
He will leverage his hands on international legal experience to conform the requirements of DCid to 
be both broadly applicable to a number of use cases, but also to have specific benefits to fit into 
regulatory norms such as KYC compliance.

**Carlos Bruguera** is a software engineer with more than 12 years of experience working on a broad 
spectrum of business areas, currently focused on _decentralized identity_ research and Ethereum 
smart contract development. His main fields of work include token economy design, self-sovereign
identity and theoretical computer science.

**Ben Gervais** is the team lead of SelfKey R&D, with extensive expertise in full-stack javascript 
development and valuable leadership skills, he's been dedicated to develop technology solutions for 
KYC and general financial compliance for the last few years. His main areas of work also include 
DeFi, artificial intelligence and crypto wallet development.


### Timeline, Milestones and Deliverables

The project will be developed divided in 2 phases as follows:

#### Phase I: DIDs

**Deliverables**:

* DID ledger smart contract
* DID resolver integrated with [DIF's universal resolver](https://github.com/decentralized-identity/universal-resolver)
* DID management javascript library
* Gnosis Safe integration tests

Time estimate: 8 weeks

Price: $24,000

#### Phase II: Verifiable Credentials

**Deliverables**:

* Verifiable Credential registry smart contract 
* Gnosis-specific credential modules
* Credential management javascript libraries
* Gnosis Safe integration tests

Time estimate: 8 weeks

Price: $24,000

### Closing thoughts

We believe Gnosis Safe is today's most flexible and advanced multi-signature platform, not only for 
Ethereum but for crypto in general and we are confident that integrating with decentralized identity
tools and standards will broaden Gnosis contracts' applicability to a vast spectrum of individual 
and corporate use cases.

The following projects are also on the roadmap if DCID is granted:

* DID authentication and communication library (implementing [DIDComm](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0005-didcomm))
* Secure Data Storage layer for identity owners to manage and share data and credentials
* Gnosis App for identity management
