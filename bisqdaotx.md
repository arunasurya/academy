# Bisq DAO Transactions

## Introduction
Bisq DAO transactions are basically Bitcoin transactions that have extra data added to them. The Bitcoin network is not aware of that data, only [the Bisq network](bisqp2p.md) is. [The Bisq software](bisqsoftware.md) contains the script for creating Bisq DAO transactions. You can read more on Bitcoin transactions [here](bitcointx.md).

## Genesis Transaction
Upon the Bisq DAO launch, Bisq developers will take the transaction output with BTC from a donation to create a new Bitcoin transaction. This transaction will be labeled on Bisq as **the genesis transaction**. While the input of this transaction is in BTC, the output is in BSQ. BSQ is [a colored coin based on Bitcoin](bsqtokens.md).

The outputs of all the subsequent transactions stemming from the genesis transaction will continue to be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label.  

## Issuance Transaction 
Except for the genesis transaction, BSQ issuance is decentralized. Any stakeholder (BSQ holder) can issue new BSQ via an issuance transaction. Decentralized issuance is accomplished in the Bisq DAO in monthly voting cycles. 

## Voting
[The Bisq voting cycle](voting.md) consists of four phases: proposal phase, blind vote, vote reveal and vote result. A stakeholder participating in each phase of the cycle creates a total of three new Bisq DAO transactions. These transactions are: a proposal transaction, a blind vote transaction and a vote reveal transaction. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html).  

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder creates a proposal transaction to make any kind of proposal such as a compensation request, listing or removing an asset on Bisq or changing a fee. The main reason for creating a proposal transaction is to have a timestamp on the Bitcoin blockchain so that the Bisq network can confirm that the transaction has indeed been made at a specific time. 

A stakeholder needs to pay a small proposal fee which discourages maliciously or carelessly overwhelming the network with meaningless transactions. Let's take a look at an example of a proposal transaction, a compensation request.

### Compensation Requests
When a contributor files a compensation request, they need to create a bitcoin transaction with the transaction input in BTC. If the compensation request is approved, that transaction is interpreted as **the issuance transaction** and its output, which was previously in BTC, is now in BSQ. That BSQ amount appears in the contributor's BSQ wallet. The Bitcoin network is not aware of this label and treats it like any other Bitcoin transaction.

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. Each vote is encrypted so that those voters who have voted earlier in the cycle do not influence those who join later. The encrypted vote is transmitted to other Bisq nodes. Once you create a blind vote transaction, you cannot change your vote since any change will result in a significant change in the encrypted message. This makes the voters commited to their votes. 

## Vote Reveal Transaction
In the vote reveal phase, a vote reveal transaction is created automatically by the Bisq software. The transaction contains a decryption key so that other nodes can read the contents of the votes. All the nodes participating in the voting need to be online to reveal their votes. 

As part of the vote reveal transaction, the hash of the voting data is published on the Bitcoin blockchain. The nodes compare the hash with their own hash to check if they had received all the votes.

