# Bisq Transactions

## Introduction
Bisq transactions are basically [Bitcoin transactions](bitcointx.md) that have some extra data added to them based on the Bisq script. 

## Genesis Transaction
Upon DAO launch, 2.5BTC (from a donation) will be used to create 2.5M BSQ  in the genesis transaction and distributed to past contributors. Since there are 100,000,000 satoshis in 1BTC, 1BSQ is equal to 100 Satoshi. The outputs of all the subsequent transactions stemming from the genesis transaction will be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label, only [the Bisq network](bisqnetworkblogpost.md).  

## Issuance Transaction 
While the genesis transaction is created only once on Bisq, any stakeholder (BSQ holder) can create a new issuance transaction. The output of the issuance transaction which is the newly colored BSQ that is accepted by the Bisq network and becomes the contributor's compensation. The Bitcoin network is not aware of this particular label and treats it like any other Bitcoin transaction. An issuance transaction is created during the Bisq voting process which happens at regular intervals.  

### Voting
[A voting cycle](voting.md) consists of four phases: proposal phase, blind vote, vote reveal and vote result. A stakeholder participating in each phase of the cycle creates a total of three new Bitcoin transactions. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html). These transactions are: a proposal transaction, a blind vote transaction and a vote reveal transaction. The proposal transaction is interpreted as the issuance transaction by the Bisq network upon approval by the stakeholders in the vote result phase.  

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder needs to create a proposal transaction to make any kind of proposal such as a compensation request, listing or removing an asset on Bisq or changing a fee. There are several reasons why a proposal transaction is needed. The first one is to have a record of that transaction on the Bitcoin blockchain so that the Bisq network can confirm that the transaction has been made and act on it. The input of the proposal transaction is plain old BTC and the output is interpreted as newly colored BSQ upon approval of the proposal. A stakeholder needs to pay a small proposal fee which keeps those who want to overwhelm the network with meaningless transactions at bay.

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. As the name suggests, the voting is done anonymously so that the earlier voters do not influence the later participants. The vote is encrypted and transmitted to other Bisq nodes. Once you create a blind vote transaction, you cannot change it.

### Vote Reveal Transaction
A vote reveal transaction is created. 

## Proposal Transaction => Issuance Transaction
In the vote result phase, the proposal transaction turns into an issuance transaction if it has been approved in the voting process. 

