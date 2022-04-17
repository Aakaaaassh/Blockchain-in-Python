# Blockchain-in-Python
Learn the fundamental concepts of Blockchain and implement them in Python.

# 1. Representing Transactions
In this lesson, you’ll build a small blockchain of your own in Python! This lesson assumes a familiarity with Python syntax, functions, loops, importing libraries, and constructing classes, but there are some hints along the way to help out. If you’ve never used Python before, you might want to learn some with Codecademy.

The blockchain is a new way of storing and moving data securely. The data mostly consists of transactions which include messages exchanged between two parties. Before we start creating our blockchain, let’s think of a way to store a transaction like the one shown below:

- amount: 30
- sender: Alice
- receiver: Bob

In this example, Alice is trying to transfer 30 units of some currency to Bob. Can you think of a Python data type to best represent the above transaction?

This transaction is best represented in the form of a Python dictionary, with keys for the required fields and values specific to the transaction.

These transactions are all stored inside the mempool, a pool of transactions that miners reference when selecting the set of transactions they want to verify.

# 2. Creating Blocks
Now let’s think of a way to represent a block in Python. We could create a bigger dictionary and store our data inside this dictionary. But since blocks can be represented as objects, let’s create a Block Class which we can easily use to create new blocks.

Recall that a Block contains the following properties:

- Timestamp
- Transaction
- Hash
- Previous Hash
- Nonce
In this exercise, we will be creating the default constructor for the Block class in our Mini-Blockchain.

# 3. Hashing and SHA-256
Before we create a more dynamic blockchain, let’s learn how to use a hash function in Python. Specifically, we will be using the SHA-256 hash function which can be easily imported in Python.

We will use the SHA-256 as a regular function that takes in a random string as its argument. To properly use this function in Python 3, our string must be encoded before being passed as an argument. To encode the string, we use the .encode() method.
