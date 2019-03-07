# Bisq DAO Transactions

## Introduction
Bisq DAO transactions are basically Bitcoin transactions that have extra data added to them. The Bitcoin network is not aware of that data, only [the Bisq network](bisqp2p.md) is. [The Bisq software](bisqsoftware.md) contains the script for creating Bisq DAO transactions. You can read more on Bitcoin transactions [here](bitcointx.md).

## Genesis Transaction
Upon DAO launch, Bisq developers will take the transaction output with a certain amount of BTC from a donation to create a new Bitcoin transaction. This transaction is labeled on Bisq as **the genesis transaction**. While the input of this transaction is in BTC, the output is in BSQ. 1 BSQ is equal to 100 satoshis. The outputs of all the subsequent transactions stemming from the genesis transaction will continue to be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label.  

## Issuance Transaction 
Except for the genesis transaction, BSQ issuance is decentralized. Any stakeholder (BSQ holder) can issue new BSQ via an issuance transaction. Decentralized issuance is accomplished in the Bisq DAO in monthly voting cycles. 

## Voting
[The Bisq voting cycle](voting.md) consists of four phases: proposal phase, blind vote, vote reveal and vote result. A stakeholder participating in each phase of the cycle creates a total of three new Bisq DAO transactions. These transactions are: a proposal transaction, a blind vote transaction and a vote reveal transaction. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html).  

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder creates a proposal transaction to make any kind of proposal such as a compensation request, listing or removing an asset on Bisq or changing a fee. There are several reasons why a proposal transaction is needed. The first one is to have a record of that transaction on the Bitcoin blockchain so that the Bisq network can confirm that the transaction has been made and act on it. A stakeholder needs to pay a small proposal fee which discourages maliciously or carelessly overwhelming the network with meaningless transactions. Let's take a look at an example of a proposal transaction, a compensation request.

### Compensation Requests
Here is an example of a proposal transaction, a compensation request. As a contributor, I file a compensation request for 1000BSQ. Since 1BSQ is worth 100 satoshis, I need to create a bitcoin transaction with the input of 100,000 satoshis (plus any transaction fees) from my Bisq BTC wallet. If the compensation request is approved, that transaction is interpreted as the issuance transaction and its output, which was previously in BTC, is now 1000BSQ which appears in my BSQ wallet. The Bitcoin network is not aware of this label and treats it like any other Bitcoin transaction.

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. Each vote is ecnrypted so that those voters who have voted earlier in the cycle do not influence those who joined later. The vote is encrypted and transmitted to other Bisq nodes. Once you create a blind vote transaction, you cannot change your vote since any change will result in a significant change in the encrypted message. This makes the voters commited to their votes.

## Vote Reveal Transaction
In the vote reveal phase, a vote reveal transaction is created automatically by the Bisq software. The transaction contains a decryption key so that other nodes can read the contents of the vote. All the nodes participating in the vote need to be online to reveal their votes. During this period, the Bisq sofware collects all the voting data in a block, hashes it and publishes the hash to all the other nodes. The nodes compare the hash with their own hash to check if they had received all the votes.

