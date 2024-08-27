# Simple Blockchain Simulation
This repository contains a simple blockchain simulation called "TestCoin." The project demonstrates the basic principles of blockchain technology, including hashing, data integrity, and the immutability of the blockchain ledger. This is a basic implementation of a blockchain structure where each block stores a set of transactions and the hash of the previous block, ensuring the chain's integrity.
## Requirements
  - Python 3
  - hashlib (comes with Python standard library)
## Project Overview
### Introduction
The TestCoin Blockchain Simulation is a Python-based project that illustrates how transactions are recorded in blocks and linked together in a blockchain. This simulation highlights the key features of a blockchain, such as hash functions, which ensure data integrity and detect any tampering attempts.
### Key Features
1. Simple Block Structure:
  - Each block contains a list of transactions and the hash of the previous block. This creates a chain of blocks where each block is dependent on the data of the previous block.
2. SHA-256 Hashing:
  - The project uses SHA-256 hashing to secure the data within each block. Any modification to the block's data will result in a completely different hash, showcasing the avalanche effect.
3. Transaction Recording:
  - Transactions are recorded in a list, and each block can store multiple transactions. These transactions are then concatenated with the hash of the previous block to form the data for the current block.
4. Block Linking:
  - The hash of each block is used as a reference in the subsequent block, ensuring that any change in a block will affect all subsequent blocks, making the blockchain immutable.
### Usage Guidelines:
1. Clone the Repository: Start by cloning the repository from GitHub to your local machine or opening it in Google Colab.
2. Running the Code: Once the script is opened in a Python environment (such as Google Colab or any Python IDE), execute the cells in order. This will generate a sequence of blockchain blocks, each containing a set of transactions and their corresponding hash values.
3. Modifying Transactions: The script allows for easy modification of transaction data. Users can experiment by altering the transaction details and re-running the script to observe how these changes impact the resulting block hashes. This demonstrates the critical concept of data integrity within a blockchain.
4. Understanding the Output: The output will display the data stored in each block and its respective hash. This will help in understanding how the blockchain maintains its security and immutability by linking blocks through their hashes.
### Avalanche Effect Demonstration:
The script also includes a demonstration of the avalanche effect, where a small change in one transaction (such as changing "Jennie sends Parker 5.1 TC" to "Jennie sends Parker 5.2 TC") results in a completely different hash for the block. This change propagates through the subsequent blocks, highlighting the sensitivity and security provided by the hashing mechanism.
### Conclusion
The TestCoin Blockchain Simulation provides a fundamental understanding of how blockchains work. By simulating transactions and block creation, the project demonstrates key blockchain principles such as data integrity, immutability, and the impact of hash functions. This basic implementation can be expanded and modified to explore more complex blockchain concepts.
