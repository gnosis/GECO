# Safe Apps Grants
### Get started building with Safe Apps and receive up to $3,000


### What are Safe Apps?


Safe Apps allow users to interact with Ethereum applications straight from the Safe Multisig interface. Users are able to customize their own interface by selecting from a list of apps. If an app is not listed in the UI by default, it’s possible to add a custom app by simply putting in the link to that app. Once apps are added, interacting with them will feel like executing any other multisig transaction. If your Safe has multiple signatures required to execute a transaction, those same requirements apply to Safe Apps. 

**We think this makes Safe Multisig a browser into the “internet of value” and we want to build this browser together with the entire Ethereum ecosystem.**

See the [Safe Apps announcement post](https://blog.gnosis.pm/introducing-gnosis-safe-apps-faef908f69c6) for more details.

### What are Safe Apps Grants?
We are introducing Safe Apps grants to incentivize the community to extend the functionality of the Safe Multisig and enable small projects or independent developers to build their first Safe App. 

### Scope

Safe Apps are a blank canvas with a lot of opportunities to build useful applications and extend the feature set of the Safe Multisig. Just a few example use-cases include:

- Swapping tokens on a decentralized exchange such as Kyber or Uniswap
- Buy cover on Nexus Mutual
- Open / manage Maker Vaults
- Register and manage ENS domains
- Mixer integration (e.g. Tornado Cash)
- ... and many more

### Who can participate?

Anyone can participate in this grant program and start building Safe Apps. However, we will only pay out grants to projects/ companies with less than 10 members. Also, we will only consider Safe Apps from projects/ teams that have not received funding from VCs or token sales.

### Grant Payouts

Grants are paid out at the sole discretion of Gnosis, with varying rewards depending on the perceived complexity of the app. As a rough heuristic, we have added the amount of work we would expect to be put into building a Safe App to achieve a specific reward level. 

### Grant Levels

**Low complexity: $750**
(1-3 days of work)

**Medium complexity: $1,500** 
(3-10 days of work)

**High complexity: $3,000**
(>10 days of work)



### Ressources

Here are a few tools and resources that will help you build your first Safe App:

* [Documentation](https://docs.gnosis.io/safe/docs/sdks_safe_apps/)
* [Safe App SDK](https://github.com/gnosis/safe-apps-sdk)
* [UI Styleguide](https://drive.google.com/file/d/18QxvqPzJ39Da3peSId0hJe9dL2mSB818/view)
* [Reusable React Components](https://components.gnosis-safe.io)
* [Safe Multisig Web Interface](https://github.com/gnosis/safe-react)

Please let us know if you have ideas to improve the developer tooling!

### How to apply for a Grant?

To ensure your Safe App is considered "valuable" by the Gnosis team, please submit your proposal beforehand here:

1. Fork the [GECO repo](https://github.com/gnosis/GECO).
1. Create a new file with your project’s name in the Proposals folder
1. Outline your proposal in that file including the use case and functionality of the Safe App (250-500 words).
1. Create a Pull Request to merge your submission into our repository.

The applications are evaluated on a rolling basis, and you can expect a decision regarding a potential grant payout within 14 days. 


### Evaluation / Requirements

In order to be eligible for a grant, a Safe App needs to fulfill the following criteria:

#### Valuable
Safe Apps that are considered for one of the above-mentioned grants, must be considered “valuable” by the Gnosis team. We want to make sure Safe Apps are built around actual use cases. This is a subjective evaluation, but factors included in the consideration are the potential size of the user base, expected transaction volume, or user experience improvements.

#### Production-ready
The Safe App must be ready to be used by actual Safe Multisig users on mainnet. In case your Safe App interacts with smart contracts, make sure they are audited and generally perceived as production-ready. Your Safe App should overall be considered “safe” and feature a decent user experience. Risks associated with the usage of the Safe App must be communicated to the user transparently.

#### Multisig-compatible
It must be possible to integrate the Safe App into the [Safe Multisig web interface](https://gnosis-safe.io/app/#/) via URL. Safe Apps must also be compatible with the asynchronous nature of a Multisig wallet. This means that they should also work considering that a) multiple people might be required to sign a transaction and b) there might be some time delay between a Safe App action being initiated and its execution on the blockchain. We highly recommend to stick to the UI Styleguide, and use the reusable React components provided in the Resources section below. 

### How to Submit the Final Safe App?

When you have finished work on the Safe App, please update your proposal with the following information:

* Link to the open-source repository including all code associated with your Safe App
* Link to a hosted version of your Safe App (ideally on IPFS)
* Walkthrough screencast of your Safe App

After your final submission, we will evaluate the Safe App, and initiate the payout of the grant. Note that there is no guarantee of a grant being paid out before your submission has been evaluated. If the submission lacks quality, Gnosis reserves the right to not pay out the grant. 

### Support

For developer support, please join the #safe channel on our [Discord](https://discord.gg/FPMRAwK).

