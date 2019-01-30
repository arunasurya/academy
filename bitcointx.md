# Bitcoin Transactions

## Transaction inputs and outputs

- a transaction has at least one input and one output; it can also have several inputs and outputs
- an unspent transaction output is called a utxo
- a utxo can be spent by using it as an input to a new transaction
- the sum of all your utxos is the sum of you all the bitcoin you own

If you want to send bitcoin to someone, you need to create a new transaction.
- you can use one of your utxos as the sole input OR
- you can use several utxos as inputs 

### Transaction outputs
Outputs can't be divided. You need to spend whole outputs. For instance, if you have a utxo of 2BTC and only want to send 1BTC to a friend, you need to use all of it as an input to a new transaction. This transaction can then have two outputs, with 1BTC each (minus the miner fee). 

A transaction output contains the following:
- value (amount in satoshis) 
- scriptPubKey or a lock script

When you create a transaction output, you set lock conditions (in the lock script). In order to spend that output, one needs to meet those lock conditions.  

### Transaction inputs

A transaction input contains the following:
- a hash of the previous transaction
- an index of the current transaction, which always starts at `0`
- scriptSig or an unlock script 

In order to spend an input of a transaction, you need to unlock it by signing with your private key.
