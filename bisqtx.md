# Bisq Transactions

## Introduction
Bisq transactions are basically [Bitcoin transactions](bitcointx.md) that have some extra data added to them based on the Bisq script. 

## Genesis Transaction
Upon DAO launch, 2.5BTC (from a donation) will be used to create 2.5M BSQ and distributed to past contributors in the genesis transaction. Since there are 100,000,000 satoshis in 1BTC, 1BSQ is equal to 100 Satoshi. The outputs of all the subsequent transactions stemming from the genesis transaction will be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label, only [the Bisq network](bisqnetworkblogpost.md).  

## Issuance Transaction 
While the genesis transaction is created only once on Bisq, any stakeholder (BSQ holder) can create a new issuance transaction. Whenever a contributor submits a compensation request, an issuance transaction is created whose output is the newly colored BSQ that is accepted by the Bisq network and becomes the contributor's compensation. The Bitcoin network is not aware of this particular label and treats it like any other Bitcoin transaction. Before taking a closer look at the issuance transaction, let me present the context within which is it created.

### Voting
[The voting cycle](voting.md) consists of four phases: proposal phase, blind vote, vote reveal and vote result. A stakeholder participating in each phase of the cycle creates a total of three new Bitcoin transactions. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html). These transactions are: a proposal transaction, a blind vote transaction and a vote reveal transaction. The proposal transaction turns into the issuance transaction upon approval by the stakeholders in the vote result phase.  

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder creates a proposal transaction. There two main reasons why a proposal transaction is needed. The first one is to prove that a specific proposal is created on a specific date and has been confirmed by the Bitcoin network. 

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. 

### Vote Reveal Transaction
A vote reveal transaction is created. 

## Proposal Transaction => Issuance Transaction
In the vote result phase, the proposal transaction turns into an issuance transaction if it has been approved in the voting process. 

