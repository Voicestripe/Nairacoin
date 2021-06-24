# Nairacoin
Digital Naira cryptocurrency for Nigeria
Revolutionizing Nigeria Financial Economy
Nairacoin will allow people in Nigeria to buy things at local grocery stores or transfer money to others with zero fees. 
Nairacoin will eliminate transaction fees associated with credit cards.
Nairacoin is simpler to set up, more efficient, long-lasting with decentralization, more flexible and accessible to unbanked individuals.
Nairacoin will be running a permissionless blockchain. Access is provided to anyone who meets the technical requirements to run a validator node in the  blockchain.
Nairacoin lockchain has the ability to scale to billions of accounts that require low latency, high-capacity storage system and high transaction throughput.













## How to run it

First, install ```requirements.txt```.

```
pip install -r requirements.txt
```

Then you have 2 options:

- Run ```miner.py``` to become a node and start mining
- Run ```wallet.py``` to become a user and send transactions (to send transactions you must run a node, in other words, you must run ```miner.py``` too)

> Important: DO NOT run it in the python IDLE, run it in your console. The ```miner.py``` uses parallel processing that doesn't work in the python IDLE.

## How this code work?

There are 2 main scripts:

- ```miner.py```
- ```wallet.py```

### Miner.py

This file is the most important. Running it will create a node (like a server). From here you can connect to the blockchain and process transactions (that other users send) by mining. As a reward for this work, you recieve some Nairacoins. The more nodes exist, the more secure the blockchain gets.

```miner.py``` has 2 processes running in parallel:

1. The first process takes care of mining, updating new blockchains and finding the proof of work.

2. The second process runs the flask server where peer nodes and users can connect to ask for the entire blockchain or sumbmit new transactions.

> Parallel processes don't run in python IDLE, so make sure you are running it from the console.



### Wallet.py

This file is for those who don't want to be nodes but simple users. Running this file allows you to generate a new address, send coins and check your transaction history (keep in mind that if you are running this in a local server, you will need a "miner" to process your transaction).
When creating a wallet address, a new file will be generated with all your security credentials. You are supposed to keep it safe.




## Contribution

Anybody is welcome to collaborate in this project. Feel free to push any pull request (even if you are new to coding). 



