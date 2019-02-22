# Bisq Transactions

## Introduction
Bisq transactions are basically [Bitcoin transactions](bitcointx.md) that have some extra data added to them based on the Bisq script. The Bitcoin network is not aware of that data, only [the Bisq network](bisp2p.md) is. 

## Genesis Transaction
Upon the DAO launch, 2.5BTC (from a donation) is used to create 2.5M BSQ in the genesis transaction and distributed to past contributors. Since there are 100,000,000 satoshis in 1BTC, 1BSQ is equal to 100 satoshis. The outputs of all the subsequent transactions stemming from the genesis transaction will be interpreted as BSQ on Bisq. The [Bitcoin network](btcnetwork.md) is not aware of this label.  

## Issuance Transaction 
Except for the genesis transaction, BSQ issuance is decentralized. Any stakeholder (BSQ holder) can issue new BSQ via an issuance transaction. Decentralized issuance is accomplished in the Bisq DAO in regular voting cycles. 

## Voting
[The Bisq voting cycle](voting.md) consists of four phases: proposal phase, blind vote, vote reveal and vote result. A stakeholder participating in each phase of the cycle creates a total of three new Bitcoin transactions. You can track these transactions on [the Bisq explorer](https://explorer.bisq.network/index.html). These transactions are: a proposal transaction, a blind vote transaction and a vote reveal transaction. The proposal transaction is interpreted as the issuance transaction by the Bisq network upon approval by the stakeholders in the vote result phase.  

## Proposal Transaction
In the proposal phase of the voting cycle, a stakeholder needs to create a proposal transaction to make any kind of proposal such as a compensation request, listing or removing an asset on Bisq or changing a fee. There are several reasons why a proposal transaction is needed. The first one is to have a record of that transaction on the Bitcoin blockchain so that the Bisq network can confirm that the transaction has been made and act on it. A stakeholder needs to pay a small proposal fee which discourages malicious or careless behavior such as overwhelming the network with meaningless transactions. Let's take a look at an example of a proposal transaction, a compensation request.

### Compensation Requests
As a contributor, I file a compensation request for 1000BSQ. Since 1BSQ is worth 100 satoshis, I need to create a bitcoin transaction with the input of 100,000 satoshis (plus any transaction fees) from my Bisq BTC wallet. If the compensation request is approved, that transaction is interpreted as the issuance transaction and its output, which was previously in BTC, is now 1000BSQ which appears in my BSQ wallet. The Bitcoin network is not aware of this label and treats it like any other Bitcoin transaction. 

## Blind Vote Transaction
Any stakeholder who wants to vote needs to create a blind vote transaction. As the name suggests, the voting is done anonymously so that the earlier voters do not influence the later participants. The vote is encrypted and transmitted to other Bisq nodes. Once you create a blind vote transaction, you cannot change it since any change will result in a significant change in the encrypted message. This makes the voters commited to their votes.

### Vote Reveal Transaction
In the vote reveal phase, a vote reveal transaction is created automatically by the Bisq software. 

## Proposal Transaction => Issuance Transaction
In the vote result phase, the proposal transaction turns into an issuance transaction if it has been approved in the voting process. 

