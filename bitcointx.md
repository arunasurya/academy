# Bitcoin Transactions

## Main Concepts

### Transaction inputs and outputs

- a transaction has at least one input and one output
- unspent transaction output is called a utxo
- a utxo can be spent by using it as an input to a new transaction
- the sum of all your utxos is the sum of you all the bitcoin you own

A transaction output contains the following:
- value or the amount of Satoshis 
- scriptPubKey or a lock script

A transaction input contains the following:
- a hash of the previous transaction
- an index of the current transaction, which always starts at `0`
- scriptSig or an unlock script 

### Public key cryptography 
