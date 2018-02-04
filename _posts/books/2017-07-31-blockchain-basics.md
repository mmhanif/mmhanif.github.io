---
layout: post
title:  "Blockchain Basics"
category: books
tags: [books, fiction, ]
---

<a target="_blank"  href="https://www.amazon.com/gp/product/1484226038/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=1484226038&linkCode=as2&tag=42models-20&linkId=5f010f14345238fc3c0bc7a743295c1d"><img border="0" src="//ws-na.amazon-adsystem.com/widgets/q?_encoding=UTF8&MarketPlace=US&ASIN=1484226038&ServiceVersion=20070822&ID=AsinImage&WS=1&Format=_SL160_&tag=42models-20" ></a><img src="//ir-na.amazon-adsystem.com/e/ir?t=42models-20&l=am2&o=1&a=1484226038" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" />

**Blockchain Basics: A Non-Technical Introduction in 25 Steps** by Daniel Drescher

*ePub [Apress]*

I haven't read a large number of Blockchain to be able to compare this with others, but I was looking for an introduction that didn't immediately dive into code or waffle-on at length about the how the technology will transform life as we know it. This book fit the bill pretty well.

The book consists of 25 steps, grouped into 5 major stages, that all together form a learning pathm which incrementally builds the reader's knowledge of the blockchain.

**Stage 1: Terminology and Technical Foundations**

*Step 1: Thinking in layers and aspects*

* Systems can be partioned into application vs implementation and functional vs non-functional aspects.
* Integrity is a major non-functional aspect, and has three major components:
	 * Data Integrity
	 * Behavioural Integrity
	 * Security
* Most software failures are the result of violated system integrity.

*Step 2: Software Architecture and it's relation to the Blockchain*

* Software architectures can be *centralized* or *distributed*.
* The blockchain is part of the implementation of a distributed software system*
* The purpose of the blockchain is to achieve and maintain the integrity of a distributed software system

*Step 3: Recognizing the potential of peer-to-peer systems*

* Peer-to-peer systems are a specific type of distributed system that allow direct interactions between contractual partners rather than indirect interactions through a middleman.

**Stage 2: Why the Blockchain is needed**

*Step 4: Discovering the core problem*

* Integrity and trust are major concerns of peer-to-peer (P2P) systems
* Major integrity threats in P2P systems are:
	* Technical failures
	* Malicious peers
* The blockchain addresses integrity of a purely distributed P2P system comprised of an unknown number of peers with unknown reliability and trustworthiness.

*Step 5: Disambiguating the term - 4 ways to define the blockchain*

* The term blockchain can be used as:
	* a name for a data-structure: data in units called blocks, connected together like a chain.
	* a name for an algorithm: the sequence of intructions that negotiated the information content of many blockchain-data-structured in a P2P system.
	* a name for a suite of technologies: a combination of blockchain data-structure, algorithm and cryptographic and security technlogies that together achieve integrity in a P2P system.
	* an umbrella term for purely distributed P2P systems with a common application area
* Managing ans clarifying ownership is the most prominent application of the blockchain, but not the only one. 
* The blockchain is a purely distributed peer-to-peer system of ledgers that utilizes a software unit that consist of an algorithm, which negotiates the informational content of ordered and connected blocks of data together with cryptographic and security technologies in order to achieve and maintain its integrity.

*Step 6: Understanding the nature of ownership*

* Proof of ownership has 3 elements:
	* Identification of the owner
	* Identification of the object being owned
	* Mapping the owner to the object
* Mapping between owners and object can be maintained in a ledger.
* Having one ledger is risky as it can be damaged, destroyed or forged.
* Can utilize a group of independent ledgers and define ownership based in that version of reality on which the majority of ledgers agree.
* The blockchain algorith is responsible for letting individual nodes in a blockchain collectively arrive at one consitent version of the state of ownership.
* Cryptography is used to ensure identity, authentication and authorization.
* Integrity in a distributed P2P system of ledgers is found in it's ability to make true statements about ownership and to ensure only the owner can transfer their property rights to others.

*Step 7: Spending Money Twice - Examining a vulnerability of distributed P2P systems*

* Double-spending can be seen as a problem of maintaining data consistency in distributed P2P systems.
* The blockchain is a means to solving the double spending problem

**Stage 3: How the Blockchain works**

*Step 8: Planning the blockchain*

* The following tasks are necessary to design a distributed P2P system of ledgers for managing ownership:
	* Describing ownership
	* Protecting ownership from unauthorized access
	* Storing transaction data
	* Preparing ledgers to be distributed in an untrustworthy environment
	* Distributing the ledgers
	* Adding and verifying new transactions to the ledgers
	* Deciding which ledgers represent the truth
	
*Step 9: Documenting Ownership*

* Transaction data provide the following information for describing a transfer of ownership:
	* An identifier of the account who initiates the transaction and is to transfer ownership to another account
	* An identifier of that account that is to receive ownership
	* The amount of the goods to be transferred
	* The time the transaction is to be done
	* A fee to be paid to the system for executing the transaction
	* A proof that the owner of the account who hands off ownership agrees with that transfer
* The complete history of transaction data is an audit trail that provides evidence of how people acquired and handed off ownership.
* Any transaction not being part of that history is regarded as if it never happened.
* A transaction is executed by adding it to the history of transaction data and allowing it to influence the result of aggregating them.
* The order in which transaction data are added to the history must be preserved in order to yield identical results when aggregating these data.
* In order to maintain integrity, only those transaction data are added to the blockchain-data-structure that fulfill the following three criteria:
	* Formal correctness
	* Semantic correctness
	* Authorization

*Step 10: Hashing Data*

* Hash functions transform any kind of data into a number of fixed length, regardless of the size of the input data.
* There are many different hash functions that differ among others with respect to the length of the hash value they produce.
* Cryptographic hash functions are an important group of hash functions that create digital fingerprints for any kind of data.
* Cryptographic hash functions exhibit the following properties:
	* Provide hash values for any kind of data quickly
	* Deterministic
	* Pseudorandom
	* One-way usage
	* Collision resistant
* Application of hash functions to data can be accomplished by using the following patterns:
	* Repeated hashing
	* Independent hashing
	* Combined hashing
	* Sequential hashing
	* Hierarchical hashing

*Step 11: Hashing in the real world*

* Hash values can be used:
	* To compare data
	* To detect whether data that were supposed to stay unchanged have been altered
	* To refer to data in a change-sensitive manner
	* To store a collection of data in a change-sensitive manner
	* To create computationally expensive tasks

*Step 12: Identifying and protecting user accounts*

* The major goal of cryptography is to protect data from being accessed by unauthorized people.
* The major cryptographic activities are:
	* Encryption: Protecting data by turning them into cypher text by utilizing a cryptographic key
	* Decryption: Turning cypher text back into useful data by utilizing a matching cryptographic key
	* Asymmetric cryptography always uses two complementary keys: cypher text created with one of these keys can only be decrypted with the other key and vice versa.
* When utilizing asymmetric cryptography in real life, these keys are typically called the public key and private key in order to highlight their role. The public key is shared with everyone, while the private key is kept secret. For this reason, asymmetric cryptography is also called public-private-key cryptography.
* There are two classical use cases of public and private keys:
	* Everyone uses the public key to encrypt data that can only be decrypted by the owner of the corresponding private key. This is the digital equivalent to a public mailbox where everyone can put letters in but only the owner can open it.
	* The owner of the private key uses it to encrypt data that can be decrypted by everyone who possesses the corresponding public key. This is the digital equivalent to a public notice board that proves authorship.
* The blockchain uses asymmetric cryptography in order to achieve two goals:
	* Identifying accounts: User accounts are public cryptographic keys.
	* Authorizing transactions: The owner of the account who hands off ownership creates a piece of cypher text with the corresponding private key. This piece of cypher text can be verified by using the corresponding public key, which happens to be the number of the account that hands off ownership.

*Step 13: Authorizing transactions*

* Digital signatures are the digital equivalent to handwritten signatures and serve two purposes:
	* Identify its author uniquely
	* State agreement of its author with the content of a document and authorize its execution
* In the blockchain, digital signatures of transactions are cryptographic hash values of transaction data encrypted with the private key that corresponds to the account that hands off ownership.
* Digital signatures in the blockchain can be trace back uniquely to one specific private key and to one specific transaction in one process.

*Step 14: Storing transaction data*

* The blockchain-data-structure is a specific kind of data structure that is made up of ordered units called blocks.
* Each block of the blockchain-data-structure consists of a block header and a Merkle tree that contains transaction data.
* The blockchain-data-structure consists of two major data structures: an ordered chain of block headers and Merkle trees.
* One can imagine the ordered chain of block headers as being the digital equivalent to an old-fashioned library card catalog, where the individual catalog cards are sorted according to the order in which they were added to the catalog.
* Having each block header referencing its preceding block header preserves the order of the individual block headers and blocks, respectively, that make up the blockchain-data-structure.
* Each block header in the blockchain-data-structure is identified by its cryptographic hash value and contains a hash reference to its preceding block header and a hash reference to the application-specific data whose order it maintains.
* The hash reference to the application-specific data is typically the root of a Merkle tree that maintains hash references to the application-specific data.

*Step 15: Using the data store - chaining blocks of data*

* The steps to be performed in order to add new transaction data to the blockchain-data-structure are:
	* Create a new Merkle tree that contains all new transaction data to be added.
	* Create a new block header that contains both a hash reference to its preceding header and the root of the Merkle tree that contains the new transaction data.
	* Create a hash reference to the new block header, which is now the current head of the blockchain-data-structure.
* Changing data in the blockchain-data-structure requires renewing all hash references starting with the one that directly points to the manipulated data and ending with the head of the whole blockchain-data-structure as well as all hash references in between them.
* The blockchain-data-structure pursues a radical all-or-nothing approach when it comes to changing its data: One either changes the whole data structure completely starting from the point that causes the change until the head of the whole chain or one better leave it unchanged in the first place.
* All half-hearted, halfway through, or partial changes will leave the whole blockchain-data-structure in an inconsistent state, which will be detected easily and quickly.
* Changing the blockchain-data-structure completely is a very elaborate process on purpose.
* The high sensitivity of the blockchain-data-structure regarding changes is due to the properties of hash references.

*Step 16: Protecting the data store - discovering the power of immutability*

* The blockchain protects the history of transaction data from manipulation and forgery by storing transaction data in an immutable data store.
* The history of a transaction is made immutable by utilizing two ideas:
	* Storing the transaction data in the change-sensitive blockchain-data-structure, which when being changed requires rewriting the data structure starting at the point that causes the change until the head of the whole chain.
	* Requiring the solution of a hash puzzle for writing, rewriting, or adding every single block header in the blockchain-data-structure.
* The hash puzzle is unique for each block header because it depends on its unique content.
* The need to rewrite the blockchain-data-structure when it is changed and the costs of doing so make it unattractive to manipulate the history of transaction data in the first place.
* Requiring the solution of a hash puzzle for every writing, rewriting or adding of block headers in the blockchain-data-structure turns is into an append-only data store.
* A block header contains at least the following data:
	* A hash reference to the header of its preceding block
	* The root of a Merkle tree that contains transaction data
	* The difficulty of its hash puzzle
	* The time when solving the hash puzzle was started
	* The nonce that solves the hash puzzle
	
*Step 17: Distributing the data store among peers*

* Computers in a distributed peer-to-peer system communicate with one another via a digital network.
* Due to the omnipresence of the Internet, it is compelling to create a distributed peer-to-peer system by connecting the individual nodes via the Internet.
* A peer-to-peer system that uses the Internet as a medium of communication is characterized by the following facts:
	* The computers are connected with one another via the Internet.
	* Each computer is identified by a unique address.
	* Each computer can disconnect and reconnect to the system at any given time.
	* Each computer independently maintains a list of peers with which it communicates.
	* Communication between nodes is based on messages.
	* Messages are sent from one node to another over the Internet by using their unique addresses.
* Due to the adversaries of networks, the communication among the nodes is characterized by the following facts:
	* Messages are not guaranteed to arrive at the addressees, but they may get lost instead.
	* Messages may arrive more than once.
	* Messages may arrive in a different order than they were sent.
* The blockchain counteracts the adversaries of communicating over an unreliable network in the following ways:
	* Messages are sent in a gossip style. Every node that receives a message will forward it to the peers it communicates with, which in turn will handle the message in the same way.
	* Duplicates of transactions or blocks are identified and filtered out based on their cryptographic hash values.
	* Each node can order the received information because transaction data and block headers contain time stamps.
* The communication among the computers that make up the peer-to-peer system serves the following three purposes:
	* Keeping existing connections alive
	* Establishing new connections
	* Distributing new information
* Forwarding ownership-related information happens on three occasions:
	* In an ongoing fashion by forwarding new transaction data and new blocks to all nodes that are connected to the system
	* As an update for nodes that reconnect to the system after being disconnected for a while
	* As part of the on-boarding procedure that transfers a copy of the whole up-to-date version of the blockchain-data-structure to the new nodes to ensure that they become full-fledged nodes after joining the system
	
*Step 18: Verifying and adding transactions*

* The blockchain-algorithm is a series of rules and instructions that governs the way in which transaction data are processed and added to the system.
* The challenge solved by the blockchain-algorithm is to keep the system open to everyone while ensuring that only valid and authorized transactions are added.
* The blockchain-algorithm utilizes the carrot-and-stick approach, combined with competition and peer control.
* The major idea of the blockchain-algorithm is to allow all nodes of the system to act as supervisors of their peers and reward them for adding valid and authorized transactions and for finding errors in the work of others.
* Due to the rules of the blockchain-algorithm, all nodes of the system have an incentive to process transactions correctly and to supervise and point out any mistakes made by the other peers.”
* The blockchain-algorithm is based on the following concepts:
	* Validation rules for transaction data and block headers
	* Reward for submitting valid blocks
	* Punishment for counteracting the integrity of the system
	* Competition among peers for earning reward based on processing speed and quality
	* Peer control
* The rules of the competition establish a two-step rhythm that governs the work of every node in the network. At any given point in time, all nodes of the system are in either of the two phases:
	* Evaluating a new block that was created by others
	* Trying hard to be the next node that creates a new block that has to be evaluated by all others
* The working rhythm is imposed by the arrival of messages at the individual nodes.
* The majority of honest nodes and their striving for reward will outweigh the attempts of dishonest nodes to counteract the integrity of the system.

*Step 19: Choosing a transaction history*

* Delays in sending new blocks across the network or two nodes creating new blocks nearly at the same time cause the blockchain-data-structure to grow into the shape of a tree or a columnar cactus with branches that arise from a common trunk that represent conflicting versions of the transaction history.
* Selecting an identical version of the transaction history is a collective decision-making problem.
* Distributed consensus is an agreement among the members of a purely distributed peer-to-peer system in a collective decision-making problem.
* The collective decision-making problem of the blockchain is characterized by the following facts:
	* All nodes operate in the identical environment, consisting of the network, nodes that maintain their individual copies of the blockchain-data-structure, and the blockchain-algorithm that governs the behavior of the nodes.
	* The decision-making problem is to select the identical transaction history across all nodes.
	* All nodes strive to maximize their individual income earned as a reward for adding new valid blocks to the blockchain-data-structure.
	* In order to achieve their goals, all nodes send their new blocks to all their peers to have them examined and accepted. As a result, each nodes leaves its individual footprint in the environment that is the collectively maintained blockchain-data-structure.
	* All nodes use the identical criterion for selecting a history of transaction data.
* The longest-chain-criterion states that each node independently chooses the path of the tree-shaped blockchain-data-structure that contains the most blocks.
* The heaviest-chain-criterion states that each node independently chooses that path of the tree-shaped blockchain-data-structure that has the highest aggregated difficulty.
* Selecting one path of the tree-shaped blockchain-data-structure has the following consequences:
	* Orphan blocks
	* Reclaimed reward
	* Clarifying ownership
	* Reprocessing of transactions
	* A growing common trunk
	* Eventual consistency
	* Robustness against manipulations
* The deeper down the authoritative chain a block is located:
	* The further in the past it was added
	* The more time has passed since its inclusion in the blockchain-data-structure
	* The more common effort has been spent on adding subsequent blocks
	* The less it is affected by random changes of the blocks that belong to the longest chain
	* The less likely it will be abandoned
	* The more accepted it is by the nodes of the system
	* The more anchored it is in the common history of the nodes
* The fact that certainty concerning the inclusion of blocks in the authoritative chain increases as time goes by and as more blocks are added eventually is called eventually consistency.
* A 51 percent attack is an attempt to gather or control the majority of the whole voting power in a collective decision-making process with the goal to turn blocks that are part of the authoritative chain into orphan blocks and establish a new authoritative chain that contains a transaction history that is more favorable from the attackers point of view.
* A 51 percent attack has the following characteristics:
	* Economically: Changing the allocation of ownership rights by changing the collective history of transaction data.
	* Decision making: Gathering the majority of voting power in order to enforce a desired result.
	* Technically: Undermining the integrity of the system.
	* Architecturally: Establish at least temporarily a hidden element of centrality that changes the state of the system.
	
*Step 20: Paying for Integrity*

* The blockchain utilizes fees for compensating its peers for contributing to the integrity of the system.
* The instrument of payment used to compensate peers has an impact on major aspects of the blockchain such as:
	* Integrity
	* Openness
	* The distributed nature
	* The philosophy of the system
	* Desirable properties of an instrument of payment for compensating peers are:
	* Being available in digital form
	* Being accepted in the real world
	* Being accepted in all countries
	* Not being the subject to capital movement restrictions
	* Being trustworthy
	* Not being controlled by one single central organization or state
* A cryptocurrency is an independent digital currency whose ownership is managed by a blockchain that uses it as an instrument of payment for compensating its peers for maintaining the integrity of the system.

*Step 21: Bringing the pieces together*

* The blockchain is a purely distributed peer-to-peer system that addresses the following aspects of managing ownership:
	* Describing ownership: History of Transaction Data
	* Protecting ownership: Digital Signature
	* Storing transaction data: Blockchain-Data-Structure
	* Preparing ledgers for being distributed: Immutability
	* Distributing ledgers: Gossip-Style Information Forwarding Through a Network
	* Processing new transactions: Blockchain-Algorithm
	* Deciding which ledger represents the truth: Distributed Consensus
* Analyzing the blockchain involves the following aspects:
	* The application goal
	* Its properties
	* Its internal functioning
* The blockchain has two application goals:
	* Clarifying ownership
	* Transferring ownership
* The blockchain fulfills its application goals while exhibiting the following qualities:
	* Highly available
	* Censorship proof
	* Reliable
	* Open
	* Pseudoanonymous
	* Secure
	* Resilient
	* Eventually consistent
	* Keeping integrity
* Internally the blockchain consists of components that are either specific or agnostic to the application goal of managing ownership.
* The application-specific components of the blockchain are:
	* Ownership logic
	* Transaction data
	* Transaction processing logic
	* Transaction security
* The application-agnostic components are:
	* The blockchain-technology-suite
	* The purely distributed peer-to-peer architecture
* The blockchain-technology-suite consists of:
	* Storage logic
	* Consensus logic
	* Data processing logic
	* Asymmetric cryptography

**Stage 4: Limitations and how to overcome them**

*Step 22: Seeing the limitations*

* The openness of the blockchain and the absence of any form of central control are the fundamentals of its functioning but can also cause limitations for its adoption.
* Major technical limitations of the blockchain are:
	* Lack of privacy
	* The security model
	* Limited scalability
	* High costs
	* Hidden centrality
	* Lack of flexibility
	* Critical size
* The most important nontechnical limitations of the blockchain are:
	* Lack of legal acceptance
	* Lack of user acceptance
	* Technical limitations of the blockchain can be overcome by improving the existing technology or by introducing conceptual changes.
	* The nontechnical limitations of the blockchain can be overcome by educational and legislative initiatives.

*Step 23: Reinventing the Blockchain*

* The blockchain inherently contains the following conflicts:
	* Transparency vs. privacy: On the one hand, transparency is needed for clarifying ownership and preventing double spending, but on the other hand, its users require privacy.
	* Security vs. speed: On the one hand, protecting the history of transaction data from being manipulated is done by utilizing the computationally expensive proof of work, but on the other hand, speed and scalability are required in most commercial contexts.
* The transparency vs. privacy conflict has its root in the allocation of reading access rights to the blockchain-data-structure.
* The security vs. speed conflict has its root in the allocation of writing access rights to the blockchain-data-structure.
* Solving the transparency vs. privacy conflict led to the following versions of the blockchain:
	* Public blockchains grant reading access and the right to create new transactions to all users or nodes.
	* Private blockchains limit reading access and the right to create new transactions to a preselected group of users or nodes.
* Solving the security vs. speed conflict led to the following versions of the blockchain:
	* Permissionless blockchains grant writing access to everyone. Every user or node can verify transaction data and create and add new blocks to the blockchain-data-structure.
	* Permissioned blockchains grant writing access only to a limited group of preselected nodes or users that are identified as trustworthy through an on-boarding process.
* Combining these restrictions pairwise led to the emergence of four different kinds of blockchains.
* Restricting reading or writing access results in consequences on the following properties of the blockchain:
	* The peer-to-peer architecture
	* The distributed nature
	* Its purpose
* The blockchain-technology-suite causes value even in restricted environments for the following reasons:
	* The number of nodes can vary due to technical failures or downtime.
	* Every distributed system faces the adversaries of networks that make communication on the level of individual messages unreliable.
	* Even an on-boarding process may not guarantee the trustworthiness of nodes at a 100 percent level.
	* Even trustworthy nodes may yield wrong results due to technical failures.

**Stage 5: Using the Blockchain, Summary and Outlook**

*Step 24: Using the Blockchain*

* The blockchain can be considered a purely distributed data store with additional properties such as being immutable, append-only, ordered, time-stamped, and eventually consistent.
* Being a generic data store means that the blockchain can store a wide range of data, which in turn makes it usable in a wide range of application areas.
* Based on its properties, we can identify the following generic-use patterns of the blockchain:
	* Proof of existence
	* Proof of nonexistence
	* Proof of time
	* Proof of order
	* Proof of identity
	* Proof of authorship
	* Proof of ownership
* Specific application areas of the blockchain that have already received attention or may receive attention in the future are:
	* Payments
	* Cryptocurrencies
	* Micropayments
	* Digital assets
	* Digital identity
	* Notary services
	* Compliance and audit
	* Tax
	* Voting
	* Record management
* When analyzing specific blockchain applications or blockchain services, some questions need to be answered:
	* What kind of blockchain is used?
	* Are the requirements for using the blockchain fulfilled?
	* What is the added value of using a purely distributed peer-to-peer system?
	* What is the application idea?
	* What is the business case?
	* How are peers compensated for contributing resources to the system?

*Step 25: Summarizing and going further*

* The blockchain has been and will continue to be the subject of further improvements and developments such as variations in its implementation, improving efficiency, improving scalability, and conceptual advances.
* Smart contracts, zero-knowledge proofs, and alternative ways to achieve consensus are major areas of conceptual advancement of the blockchain.
* Besides it technical merits, the blockchain may be honored for the following long-term accomplishments:
	* Disintermediation
	* Automation
	* Standardization
	* Streamlining processes
	* Increased processing speed
	* Cost reduction
	* Shift toward trust in protocols and technology
	* Making trust a commodity
	* Increased technology awareness
* Possible disadvantages of the blockchain are:
	* Lack of privacy
	* Loss of personal responsibility
	* Loss of jobs
	* Reintermediation
* Possible usages of the blockchain to be seen in the future are:
	* Limited enthusiast projects
	* Large-scale commercial projects
	* Governmental projects
