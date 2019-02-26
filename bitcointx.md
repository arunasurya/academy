# Bitcoin Transactions

## Main Concepts

### Transaction inputs and outputs

- a transaction has at least one input and one output; it can also have several inputs and outputs
- an unspent transaction output is called a utxo
- a utxo can be spent by using it as an input to a new transaction
- the sum of all your utxos is the sum of you all the bitcoin you own

If you want to send bitcoin to someone, you need to create a new transaction.
- you can use one of your utxos as the sole input OR
- you can use several utxos as inputs 


A transaction output contains the following:
- value or the amount of Satoshis 
- scriptPubKey or a lock script

A transaction input contains the following:
- a hash of the previous transaction
- an index of the current transaction, which always starts at `0`
- scriptSig or an unlock script 

## What is a Bitcoin transaction?
A Bitcoin transaction consists of inputs and outputs. A transaction references the output of the previous transaction in its input. If you want to spend bitcoin, you need to create a new transaction. It can have only one input or several inputs, depending on how much bitcoin you want to spend.

An unspent transaction output, or utxo. A utxo can be spent by using it as an input to a new transaction.   The sum of all your utxos is the sum of you all the bitcoin you own. You need to spend the entire utxo. You can use one of your utxos as the sole input to the new transaction or you can use several utxos as several inputs. When you create a transaction, you specify a lock script that, if unlocked, releases the bitcoin.


### Public key cryptography 

- a private-public key pair is needed to send and receive bitcoin
- the public key is generated from the private key 
