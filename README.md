# What is Blockchain? 
* Ever wonder how Bitcoin (and other cryptocurrencies) actually work by 3Blue1Brown?
https://youtu.be/bBC-nXj3Ng4 
* Le Bitcoin et la Blockchain (avec Heu?Reka) — Science étonnante #31 
https://youtu.be/du34gPopY5Y

```
Need to register the transaction 
--------------------------------
-Simple ledger hosted on a website
...But how to secure this ledger? 
->to secure the simple ledger : add a digital signature but easy reproductable by a computer.

Need to secure the transaction 
------------------------------
-To secure the process and prevent fraud : invention of the private (sk) and public key (pk). 256 bit signature. 
-Two functions sign and valid : 
function sign (Message with a unique ID, sk) = Signature
function valide (Message, Signature,pk) = T/F 
....But what happen if people refuse to pay their debt? 
->they add the historic of the transaction and reduce the risk of debt. 
->Bitcoin is a Ledger, the history of the transaction is the currency. 

Need to invent a broadcast transaction protocol 
-----------------------------------------------
-Duplication of the ledger : people has its own ledger on its own website hosted on its own server. 
....But is every transaction are recorded simultaneously and in the same order? 
-> Bitcoin Protocol to broadcast transaction : computational work 
Main tool : Cryptographic hash functions 

How hash function (SHA256) is working ? 
--------------------------------------
input : message  (proof of work to find with computational effort)
output : string 

SHA256("Message/ file") => produce a string of 256 bits (hash or digest)
-if you change the inputs a new hash or digest is produce randomly. 
-cryptographic ~ inverse is infeasible. Its not possible to find the message from the string of bits. 

Blockchain  (15')
-----------
-Organize Ledger in blocks of transactions chained. 
-Each block has a proof of work. A block is valid if he has a proof of work. 
-Each Leadger is passed into a SHA256 and produce a hash 
-Computational problem : for example to find what can be the input of the hash function if the 30 or 60 first bits = 0 ? 
-The first miner (computing power) to find the solution (the proof of work) validate its block and add it to the blockchain. 
One block is generated every 10 minutes. 
-The previous hash is transmitted to the next block. 
-Its impossible to change a past transaction without changing all the 
following hash generated and re-doing all the computational work to validate the hash. 
```

# Blockchain and AI 
* Blockchain Consensus Algorithms and Artificial Intelligence by Siraj Raval: https://youtu.be/5Tr13l0O1Ws 
* Openmined : Decentralized Marketplace for Data :  https://youtu.be/HAC6sqq7_-U 
* OpenMined Introduction : https://youtu.be/sXFmKquiVnk
* NumerAI : Decentralized AI Hedge Fund: https://medium.com/numerai
* Near future Self Driving Car Network : http://bit.ly/2zZeAlb

# Distributed concensus algorithms 
* Code of the proof of work algorithm on GitHub: http://bit.ly/2jcRfSZ
* Others algorithm Proof of stake Proof of activity Proof of burn : https://www.coindesk.com/short-guide-blockchain-consensus-protocols/

```
4 steps to validate a transaction 
---------------------------------
-A miner retrieve group of transactions from pending transactions to be validated 
-process work to generate proof (solve the algorithm)
-broadcast the proof of work to all nodes 
-write transactions into the blockchain if proof of work is valid for the majority of nodes 
```
