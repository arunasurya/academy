# Bitcoin Transactions

## Transaction inputs and outputs

- a transaction has at least one input and one output; it can also have several inputs and outputs
- an unspent transaction output is called a utxo
- a utxo can be spent by using it as an input to a new transaction
- the sum of all your utxos is the sum of you all the bitcoin you own

If you want to send bitcoin to someone, you need to create a new transaction.
- you can use one of your utxos as the sole input if that utxo amount is adequate OR
- you can use several utxos as inputs if each utxo is too small 

### Transaction outputs
Outputs can't be divided: you need to spend whole outputs.

Example: Alice has 2BTC in one utxo. If she wants to send 0.5BTC to Bob, she needs to take the entire utxo of 2BTC, send 0.5BTC to Bob and the remainder (1.5BTC) as a change to her new address (minus the miner fee).  

A transaction output contains the following:
- value (amount in satoshis) 
- scriptPubKey or a lock script

When you create a transaction output, you set lock conditions (in the lock script). In order to spend that output, one needs to meet those lock conditions. A typical lock condition is as follows:
- here is a hash of the public key. 
- provide a public key that hashes to that value as well a digital signature. 

You can mathematically prove that a certain private key that has that corresponding public key was used to create the signature. A message you are signing with your private key is the entire transaction (without the signature).

### Transaction inputs

A transaction input contains the following:
- a hash of the previous transaction
- an index of the current transaction, which always starts at `0`
- scriptSig or an unlock script 

In order to spend an input of a transaction, you need to unlock it by signing with your private key.

In order to use utxos as inputs to a new transaction, you need to provide an unlock script, that when run together with a lock script of that output, validates. 
