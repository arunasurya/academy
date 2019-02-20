# Bisq Transactions

## Introduction
Bisq transactions are basically [Bitcoin transactions](bitcointx.md) that have some extra data added to them based on the Bisq script. 

## Genesis Transaction
Upon DAO launch, 2.5BTC (from a donation) will be used to create 2.5M BSQ in the genesis transaction. Since there are 100,000,000 satoshis in 1BTC, 1BSQ is equal to 100 Satoshi. The outputs of all the subsequent transactions stemming from this genesis transaction will be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label, only [the Bisq network](bisqnetworkblogpost.md).  

## Issuance Transaction 
Whenever a contributor submits a compensation request, an issuance transaction is created, whose output is new BSQ that is accepted by the Bisq network. The Bitcoin network is not aware of this particular label and treats it like any other Bitcoin transaction. Let's take a look at the specifics of the issuance transaction.

### Voting
The voting cycle consists of four phases: proposal phase, blind vote, vote reveal and vote result. Each voting cycle will last a total of 30 days and a total of 4380 blocks. A stakeholder participating in each phase of the cycle creates a total of three new bitcoin transactions which appear on the Bitcoin blockchain. Let's take a look at each of these transactions in more detail. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html).

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder creates a proposal transaction. 

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. 

### Vote Reveal Transaction
A vote reveal transaction is created. 

## Issuance Transaction = Proposal Transaction
In the vote result phase, the proposal transaction turns into an issuance transaction if it has been approved in the voting process. 

