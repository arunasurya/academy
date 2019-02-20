# Bisq Transactions

## Introduction
Bisq transactions are basically [bitcoin transactions](bitcointx.md) that have some extra data added to them based on the Bisq script. 

## Genesis Transaction
2.5BTC (from a donation) will be used to create 2.5M BSQ in the genesis transaction upon the DAO launch. Since there are 100,000,000 satoshis in 1BTC, 1BSQ is equal to 100 Satoshi. 

## Issuance Transaction 
Whenever a contributor submits a compensation request, they create an issuance transaction whose output is new BSQ that is accepted by the network.

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

