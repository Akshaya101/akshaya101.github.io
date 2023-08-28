---
title: "Cryptography : The Corestone Behind Blockchain Technology"
date: 2023-08-23T20:25:10+05:30
description: 'This article gives you an idea about the basics of cryptography, types of cyrptography, cyrptographic algorithms like SHA-256, ZKPs and much more.'
ShowBreadCrumbs: true
ShowToc: true
TocOpen: false
cover:
    image: "images/Cryptography.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
---
### Introduction

Blockchain is one of the most trending and trustworthy technologies in current times, allowing businesses and individuals to maintain an unchangeable record of events, providing insights into the maintenance and lifecycle of a product.

The reason why blockchain is so popular is because of its features, such as providing security, maintaining data integrity, and building a tamper-proof system. All these features in blockchain are due to the cryptographic algorithms implemented at the core of the technology.

---

### **What is Cryptography?**

**Cryptography** can be defined as the study and practice of sending secure, encrypted methods that are implemented during the communication process between two or more parties. The word **“Crypto”** stands for “**concealed or secret”,** so cryptography can also be defined as the analysis and deciphering of **“secret messages”** between two parties.

Depending upon the configuration and the algorithms that are implemented cryptography can either involve pseudo or full anonymity. During a transaction, the sender **“encrypts”** the message with the help of different types of cryptographic algorithms making it inaccessible to third-party applications and the receiver **“decrypts”** the message with the necessary verification methods.

### **Terms related to Cryptography :**

* **Encryption:** It is a process of plaintext (normal text) to a ciphertext (random sequence of bits).
    
* **Decryption:** The inverse process of encryption, conversion of ciphertext to plaintext.
    
* **Cipher:** The mathematical function, i.e. a cryptographic algorithm which is used to convert plaintext to ciphertext.
    
* **Key:** A small amount of information is required to induce the output of the cryptographic algorithm.

---

### **Types of Cryptography :**

There are different practices in which a message can be encrypted and decrypted. We will look into some of the popular types of cryptographic practices that influence the working of Blockchains.

1. **Public-Key Cryptography (Asymmetric Cryptography):**
    
    1. This type is used for creating secure addresses, verifying digital signatures, and enabling secure communication between participants in the blockchain network. It involves using a pair of keys: a public key for encryption and a private key for decryption and signing.
        
    2. Popular Blockchains such as Bitcoin, and Ethereum use these algorithms to ensure cryptographic transactions and address generation.
        
2. **Hash Functions:**
    
    1. Hash functions are used to create unique identifiers for blocks, transactions, and data. They help maintain data integrity by ensuring that even a small change in the input data results in a completely different hash output.
        
    2. Hash functions secure transactions and create block identifiers. Each block's hash includes the hash of the previous block, forming the blockchain. Such types of Hash functions are implemented in Blockchains like Bitcoin.
        
3. **Digital Signatures:**
    
    1. Digital signatures are crucial for verifying the authenticity of transactions and messages within the blockchain. They ensure that transactions are valid and have been approved by the rightful owner of the private key.
        
    2. The digital signatures are a part of the transaction starting from verification, authentication and secure inclusion of the transaction into the block. A detailed explanation of how it is carried out is given below :
        
        1. **Transaction Verification:**
            
            * Users generate a pair of cryptographic keys: a private key kept secret and a corresponding public key shared openly.
                
            * When initiating a transaction, the transaction details are hashed.
                
            * The private key is used to digitally sign the hash, generating a unique digital signature.
                
        2. **Transaction Authentication:**
            
            * The transaction, along with the digital signature, is broadcast to the network.
                
            * Nodes verify the signature's authenticity using the sender's public key and ensure the transaction's integrity.
                
        3. **Secure Inclusion in Blocks:**
            
            * In Bitcoin, miners compete to validate transactions and create new blocks by solving computational puzzles (Proof of Work).
                
            * In Ethereum, validators (Ethereum 2.0's Proof of Stake) propose and validate blocks.
                
4. **Consensus Mechanisms:**
    
    1. Consensus Mechanisms can be defined as the protocols and algorithms that ensure agreement among participants in a distributed network, like a blockchain, about the state of the shared data or the validity of transactions.
        
    2. Types of Consensus Mechanisms are Proof of Work, Proof of Stake and Proof of Authority.
        
5. **Ring Signatures:**
    
    1. Ring signatures enable a user to sign a message on behalf of a group without revealing which member signed. This adds a layer of privacy to transactions.
        
    2. Monero, a type of Blockchain, uses ring signatures to enhance transaction privacy. Ring signatures create a group of possible signers, making it difficult to determine the actual sender.

---

### Types of Cryptographic algorithms used in different Blockchains :

To understand the working on Blockchain on a base level, it is necessary to know about the type of algorithms that are implemented in different blockchains.

1. **SHA-256**
    
    1. SHA stands for “Secure Hash Algorithm”. The main objective of this algorithm is to generate a hash from the given input. After multiple mathematical and logical operations, a unique 256-bit hash value is generated. The resulting output is always of the same length (256-bit). SHA-256 is a one-way function, meaning it's computationally infeasible to reverse-engineer the original input from the hash.
        
    2. In blockchains like **Bitcoin**, SHA-256 is used to create the cryptographic hash of a block's header, which includes previous block hashes, transaction data, and other information.
        
2. **Elliptic Curve Digital Signature Algorithm**
    
    1. ECDSA is a widely used cryptographic algorithm that provides a way to create digital signatures, which are used to verify the authenticity and integrity of messages, transactions, and data in various applications, including blockchain technology.
        
    2. ECDSA plays a significant role in many blockchain networks, including **Bitcoin and Ethereum**, where it's used to create and verify digital signatures for transactions and other blockchain operations.
        
3. **Zero Knowledge Proofs**
    
    1. Zero-Knowledge Proofs (ZKPs) are cryptographic protocols that enable one party (the prover) to prove to another party (the verifier) that a statement is true without revealing any specific information about the statement itself.
        
    2. ZKPs can be used to prove the validity of transactions, the execution of smart contracts, and other computations without exposing sensitive data. This is particularly valuable in preserving privacy while ensuring trust in blockchain systems.
        

Other types of Cryptographic algorithms relevant to Blockchains are Keccak-256 (used in Ethereum), RSA, ECC (Elliptic Curve Cryptography), and AES (Advanced Encryption Standard).

---

### Significance of Cryptography in Blockchain Development :

1. **Enhancing Data Security:**
    
    * Cryptography secures data by transforming it into unreadable code that can only be decrypted with the correct key. In blockchain, this prevents unauthorized access and tampering of sensitive information, ensuring the reliability of transactions and records.
        
    * Example: Cryptographic encryption ensures that a financial transaction's details, such as sender, receiver, and amount, are concealed from potential eavesdroppers, protecting users' privacy.
        
2. **Verifying Transaction Authenticity:**
    
    * Digital signatures use cryptographic techniques to validate the authenticity of transactions. This prevents unauthorized alterations and ensures that transactions come from legitimate sources.
        
    * Example: When a user initiates a cryptocurrency transfer, their private key generates a digital signature. Recipients can use the sender's public key to verify the signature, confirming the transaction's origin.
        
3. **Preserving User Privacy:**
    
    * Cryptography, such as zero-knowledge proofs, allows users to prove the validity of a statement without revealing the actual data, ensuring transaction confidentiality.
        
    * Example: Zero-knowledge proofs in a blockchain-based medical records system enable patients to prove they have specific health conditions to insurance providers without disclosing their full medical history.
        
4. **Data Integrity and Immutability:**
    
    * Hash functions generate unique identifiers for data, which change even with the smallest alteration. This makes it impossible to modify data without detection, ensuring the integrity of blockchain records.
        
    * Example: In a supply chain blockchain, each change of ownership is hashed and added to the blockchain. If anyone tries to modify a record, the hash would change, indicating tampering.
        
5. **Smart Contracts and Secure Execution:**
    
    * Cryptography ensures the secure execution of smart contracts by verifying the conditions and participants' identities, preventing unauthorized execution.
        
    * Example: A smart contract in a decentralized marketplace executes a transaction only if the buyer's digital signature and payment are valid, ensuring both parties fulfill their obligations.

---

### Conclusion

Cryptography is one of the most prominent bases for the existence of technologies like Blockchain, which is situated on the pillars of data integrity, data security, decentralization, and secure communication. These pillars offer a chance, for the first time, to witness a transparent, open, and trustworthy communication network.

---

Here are a few resources that helped me to understand more about Cryptography :

📖 **Something to Read**
- [What is Cryptography? ](https://www.coinbase.com/learn/crypto-basics/what-is-cryptography)
- [Introduction to Blockchain](https://brave.com/web3/intro-to-blockchain/#what-is-blockchain-technology)
- [Introduction to Web3](https://ethereum.org/en/web3/)

🎬 **Something to Watch**
- [Blockchain 101 - A Visual Demo](https://www.youtube.com/watch?v=_160oMzblY8)
- [Blockchain & Smart contracts: Digital Evolution Conference 2018](https://www.youtube.com/watch?v=HNCwbKAY7AM)

🎙️ **Something to Listen**
- [What is Blockchain and How does Blockchain Technology Work?](https://open.spotify.com/episode/4vQ9O9XMTYd1AFz0VxaWuj?si=sx2KlsLYQU-wh3gZRz8PDw)
- [Security. Cryptography. Whatever.](https://open.spotify.com/show/0bMJ5a7e4er7yDHMuGs9jp)

