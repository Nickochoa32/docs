# Consensus

When it comes to blockchains like Ethereum, which are, in essence, distributed databases, the network's nodes must reach an agreement on the network's current state. This agreement is achieved using consensus mechanisms.

Although consensus mechanisms aren't directly related to building a dapp, understanding them will illuminate concepts relevant to you and your users' experience, like gas prices and transaction times.

## Prerequisites

---

To better understand this page, we recommend you first read our introduction to Ethereum.

## What is consensus?

---

By consensus, we mean that a general agreement has been reached. Consider a group of five people going to the cinema. If three out of five agree on a film, a consensus is achieved — majority rules.

In regards to blockchain, reaching consensus means that at least 51% of the nodes on the network agree on the next global state of the network.

## What is a consensus mechanism?

---

Consensus mechanisms (also known as consensus protocols or consensus algorithms) allow distributed systems (networks of computers) to work together and stay secure.

For decades, these mechanisms have been used to establish consensus among database nodes, application servers, and other enterprise infrastructure. In recent years, new consensus mechanisms have been invented to allow cryptoeconomic systems, such as Ethereum, to agree on the state of the network.

A consensus mechanism in a cryptoeconomic system also helps prevent certain kinds of economic attacks. In theory, an attacker can compromise consensus by controlling 51% of the network. Consensus mechanisms are designed to make this "51% attack" unfeasible. Different mechanisms are engineered to solve this security problem in different ways.


## Types of consensus mechanisms

---

### Proof-of-work

Ethereum, like Bitcoin, currently uses a proof-of-work (PoW) consensus protocol.

#### Block creation

Proof-of-work is done by miners, who compete to create new blocks full of processed transactions. The winner shares the new block with the rest of the network and earns some freshly minted ETH. The race is won by whosever computer can solve a math puzzle fastest – this produces the cryptographic link between the current block and the block that went before. Solving this puzzle is the work in "proof-of-work".

#### Security

The network is kept secure by the fact that you'd need 51% of the network's computing power to defraud the chain. This would require such huge investments in equipment and energy; you're likely to spend more than you'd gain.

More on proof-of-work

### Proof-of-stake

Ethereum has plans to upgrade to a proof-of-stake (PoS) consensus protocol.

#### Block creation

Proof-of-stake is done by validators who have staked ETH to participate in the system. A validator is chosen at random to create new blocks, share them with the network and earn rewards. Instead of needing to do intense computational work, you simply need to have staked your ETH in the network. This is what incentivises healthy network behaviour.

#### Security

A proof-of-stake system is kept secure by the fact that you'd need 51% of the total staked ETH to defraud the chain. And that your stake is slashed for malicious behaviour.

More on proof-of-stake

### A visual guide

Watch more on the different types of consensus mechanisms used on Ethereum:


### Sybil resistance & chain selection

Now technically, proof-of-work and proof-of-stake are not consensus protocols by themselves, but they are often referred to as such for simplicity. They are actually Sybil resistance mechanisms and block author selectors; they are a way to decide who is the author of the latest block. It's this Sybil resistance mechanism combined with a chain selection rule that makes up a true consensus mechanism.

Sybil resistance measures how a protocol fares against a Sybil attack. Sybil attacks are when one user or group pretends to be many users. Resistance to this type of attack is essential for a decentralized blockchain and enables miners and validators to be rewarded equally based on resources put in. Proof-of-work and proof-of-stake protect against this by making users expend a lot of energy or put up a lot of collateral. These protections are an economic deterrent to Sybil attacks.

A chain selection rule is used to decide which chain is the "correct" chain. Ethereum and Bitcoin currently use the "longest chain" rule, which means that whichever blockchain is the longest will be the one the rest of the nodes accept as valid and work with. For proof-of-work chains, the longest chain is determined by the chain's total cumulative proof-of-work difficulty.

The combination of proof-of-work and longest chain rule is known as "Nakamoto Consensus."

Eth2 (the beacon chain) uses a consensus mechanism called Casper the Friendly Finality Gadget, which is proof-of-stake based.

## Further reading

---

- What Is a Blockchain Consensus Algorithm?
- What is Nakamoto Consensus? Complete Beginner’s Guide
- How Does Casper work?
- On the Security and Performance of Proof of Work Blockchains

Know of a community resource that helped you? Edit this page and add it!

## Related topics

---

- Proof of work
- Mining
- Proof of stake
