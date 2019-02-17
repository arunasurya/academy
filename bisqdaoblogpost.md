## Bisq DAO: an overview

## Introduction
In my previous post, I talked about the Bisq network. This post gives you an overview of the Bisq DAO, a decentralized way of governance and decision-making.

## Bisq DAO
It is clear that the Bisq users benefit by being able to trade in a secure way without compromising their privacy. In order to continue maintaining and improving Bisq in a sustainable way, the contributors need to get paid for their work. The Bisq DAO (Decentralized Autonomous Organization) is an effective approach to align the contributors' incentives with those of the users in a self-contained and decentralized way. Its purpose is to transfer the Bisq revenue in form of the trading fees from the users to the contributors. It is based on Bitcoin and is implemented directly in the Bisq app which means that any Bisq node becomes part of the Bisq DAO. Let us take a closer look at the Bisq DAO, starting with its participants.

## Bisq Participants
The main participants in Bisq are users, arbitrators and contributors. A user is anyone who trades on Bisq. An arbitrator is a person who solves any trading disputes between trading partners. A contributor is anyone who provides valuable work for Bisq. You can become a contributor by doing some important work and then filing a compensation request. You can choose a specific role from a list of [roles](https://docs.bisq.network/roles.html) such as maintainers, operators and administrators. You are also free to define your own role that suits your background and strengths. You decide your own working schedule, the amount of work you do in a given period and how frequently you want to contribute. Some roles require consistent contributions while others are more flexible.

At this point, you may wonder if the contributors and arbitrators ever get paid for their work. They do. They get compensated for their work in BSQ tokens.

### BSQ Token
At the heart of the Bisq DAO is the BSQ token. The BSQ token is a colored coin based on the Bitcoin blockchain. The Bisq app contains the script for coloring and uncoloring the tokens. In addition to the BTC wallet, the app also has a BSQ wallet. There are two ways of issuing the BSQ tokens: through the genesis transaction and through decentralized issuance.

#### Genesis Transaction
Upon the Bisq DAO, the Bisq developers will create a bitcoin transaction and label it in the Bisq source code as the genesis transaction. The Bisq network will be aware of this label while the Bitcon network will not differentiate it from any other bitcoin transaction. All the subsequent outputs stemming from this transaction will now be colored on the Bisq network. 

You may know that a bitcoin transaction consists of inputs and outputs. A sum of all unspent transaction outputs (utxo) is the amount of bitcoin you own. The genesis transaction will take a utxo of 2.5BTC (from a donation) as its input to create 2.5M BSQ in its outputs to be distributed to past contributors. Since there are 100M satoshis in 1BTC, each BSQ is equal to 100 satoshis. The value of a BSQ token will be primarily determined by market forces but it cannot be any lower than the amount of bitcoin it is based on.

#### Decentralized Issuance
Any contributor can issue new BSQ by filing a compensation request at the end of each month for the work done in the prevous month. Let me give you an example: I file a compensation request for 1000BSQ. Since 1BSQ is worth 100 satoshis, I need to create a bitcoin transaction with the input of 100,000 satoshis (plus any transaction fees) from my Bisq BTC wallet. If the compensation request is approved, that transaction is interpreted as an issuance transaction and its output, which was previously in BTC, is now 1000BSQ.

The amount of the compensation request is determined by how much value that work has added to Bisq. Additional parameters such as an hourly market rate can also be taken into account in determining the amount, but the important point is that the work has to be complete and useful. The contributors are encouraged to break down their work into smaller chunks that can be finished within a month. It is the result that counts, not the process.

It is important to clarify that as of this moment the Bisq DAO has not been launched yet. Any revenue generated from Bisq trades goes to the arbitrators while the contributors are not being paid yet. They can still submit compensation requests for the work they have done, and the amount of their compensation is tracked on a spreadsheet. They will be paid the earned BSQ amount upon the DAO launch. 

#### Uncoloring BSQ Tokens
While new BSQ is created via the genesis transaction and issuance transactions, it can be burned or uncolored in several ways. These include various fees such as trading and voting fees and burned bonds (see below). The uncolored BSQ turns back into BTC which is used as miners' fees. 

### BSQ Supply
There will be an initial supply of 2.5M BSQ from the genesis transaction. The subsequent supply will depend on the amount of compensation requests and the usage of BSQ in the form of trading fees. The compensation requests will increase the BSQ supply while the trading fees will lead to its decrease. Currencly, around 50,000 new BSQ is issued every month since October 2017.

### Trading Fees
In the future, users will be able to buy BSQ tokens and use them as trading fees which will be heavily discounted compared to current trading fees in BTC. Instead of being directly distributed among the contributors, the trading fees will be uncolored which will lead to the decrease in the total BSQ supply. This means that each BSQ will gain in value which is beneficial for all stakeholders.

### Stakeholders
Anyone who holds BSQ tokens is considered a stakeholder. As of this moment, the only way to obtain the tokens is by being a contributor. Thus, those who have contributed most to Bisq have the proportionate amount of the BSQ tokens. 

The stakeholders are incentivized to maintain Bisq and to participate in its governance to ensure the success of the project. They have the power to decide how many new tokens are issued every month by voting on compensation requests. They also decide if a project should be prioritized or discarded, to increase or decrease various fees, etc.

### Voting
Once a contributor submits their compensation request, any stakeholder can vote on that request. This includes the contributor submitting the request if they hold any BSQ. The voting weight for each stakeholder is determined by the amount of BSQ stake used in the voting period. You can either upvote, downvote or place a neutral vote for that request. The stakeholders can also vote on other proposals such as reimbursement requests or proposals to add or remove an asset on the exchange. The stakeholders are encouraged to take voting seriously and need to pay a small voting fee in BSQ which gets uncolored. 

### Bonding
Some high stake roles such as maintainers, seed node operators or price node operators, require a bond in BSQ for the period of exercising that role. This is done as an insurance against any rogue behavior from those role holders. In the event of defection, that bond is burned, i.e., that BSQ amount is uncolored. This decreases the total supply of BSQ which is beneficial for all stakeholders. This should happen rarely and should not significantly affect the BSQ supply. 

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/).
