# A comprehensive overview of Bisq

## Introduction
If you are into cryptocurrencies, you may be interested in Bisq, a decentralized exchange that enables you to trade bitcoin for fiat currencies and other cryptocurrencies. In this post, I will give you an overview of Bisq, including the Bisq app, the Bisq network and its participants. I will also introduce the concept of the Bisq DAO, a decentralized way of governance and decision-making.   

## Bisq App
Bisq is decentralized, meaning that the exchange data such as the order book is not stored on a central server. If you want to trade, it is easy to download and install [the Bisq app](https://bisq.network/downloads/) on your computer. The Bisq app is free/open-source software (FOSS) which is maintained and improved by a group of contributors. By running the app, your computer becomes part of the Bisq network. There is no need for registration or approval from any central authorities, you just download and start the app. The app contains an internal BTC wallet.

Since its launch in April 2016, Bisq (which used to be called Bitsquare) has been providing free exchange services nonstop with the median monthly growth in trades of 50%. (TODO: add more)

There are many different payment methods that you can use on Bisq. For instance, if you are using MoneyGram to receive USD in exchange for BTC, you need to add information about your MoneyGram account so that your trading partner can send you USD. Bisq does not automatically send the USD from your trading partner to you, it just gives them the information they need to send USD to your MoneyGram account. Since your data is stored locally on your computer, the rest of the network doesn't know the details about your MoneyGram account.


## Bisq Network
The Bisq network consists of nodes running the Bisq software. Just like the Bitcoin network, it is a peer-to-peer (P2P) network that does not have a central server and is instead made up of individual peers. Some of the Bisq nodes may also be full Bitcoin nodes, typically running the Bitcoin Core software. There are public Bitcoin nodes that are run by some contributors. Upon starting, the Bisq app connects to these nodes. If there is a local Bitcoin full node, the Bisq app automatically detects it and connects to it instead. 

In addition to Bisq nodes, the network includes several other nodes, each with a specific function. Every time the Bisq app gets started, it gets connected to seed nodes. Seed nodes run the Bisq software, and they introduce users to other Bisq nodes. Price nodes fetch data on cryptocurrency prices and serve it to Bisq nodes. Currently, the price nodes fetch this data from a single centralized website, bitcoinaverage.com.

## Bisq Participants
The main participants in Bisq are users, arbitrators and contributors. A user is anyone who trades on Bisq. An arbitrator is a person who solves any trading disputes between trading partners. A contributor is anyone who provides valuable work for Bisq. You can become a contributor by doing some important work and then filing a compensation request. You can choose a specific role from a list of [roles](https://docs.bisq.network/roles.html) such as maintainers, operators and administrators. You are also free to define your own role that suits your background and strengths. You decide your own working schedule, the amount of work you do in a given period and how frequently you want to contribute. Some roles require consistent contributions while others are more flexible.

At this point, you may wonder if the contributors and arbitrators ever get paid for their work. They do. This brings us to a unique way Bisq governs itself and rewards its contributors, the Bisq DAO.

## Bisq DAO
It is clear that the Bisq users benefit by being able to trade in a secure way without compromising their privacy. In order to continue maintaining and improving Bisq in a sustainable way, the contributors need to get paid for their work. The Bisq DAO (Decentralized Autonomous Organization) is an effective approach to align the contributors' incentives with those of the users in a self-contained and decentralized way. Its purpose is to transfer the Bisq revenue in form of the trading fees from the users to the contributors. It is based on Bitcoin and is implemented directly in the Bisq app which means that any Bisq node bbecomes part of the Bisq DAO. Let us take a closer look at the Bisq DAO, starting with the BSQ Token.

### BSQ Token
At the heart of the Bisq DAO is the BSQ token. The BSQ token is a colored coin based on the Bitcoin blockchain. The Bisq app contains the script for coloring and uncoloring the tokens. In addition to the BTC wallet, the app also has a BSQ wallet. There are two ways of issuing the BSQ tokens: through the genesis transaction and through decentralized issuance.

#### Genesis Transaction
Upon the Bisq DAO, the Bisq developers will create a bitcoin transaction and label it in the Bisq source code as the genesis transaction. The Bisq network will be aware of this label while the Bitcon network will not differentiate it from any other bitcoin transaction. All the subsequent outputs stemming from this transaction will now be colored on the Bisq network. 

You may know that a bitcoin transaction consists of inputs and outputs. A sum of all unspent transaction outputs (utxo) is the amount of bitcoin you own. The genesis transaction will take a utxo of 2.5BTC (from a donation) as its input to create 2.5M BSQ in its outputs to be distributed to past contributors. Since there are 100M satoshis in 1BTC, each BSQ is equal to 100 satoshis. The value of a BSQ token will be primarily determined by market forces but it cannot be any lower than the amount of bitcoin it is based on.

#### Decentralized Issuance
Any contributor can issue new BSQ by filing a compensation request at the end of each month for the work done in the prevous month. Let me give you an example: I file a compensation request for 1000BSQ. Since 1BSQ is worth 100 satoshis, I need to create a bitcoin transaction with the input of 100,000 satoshis from my Bisq BTC wallet. If the compensation request is approved, that transaction becomes an issuance transaction the output of which will be colored as 1000BSQ and transferred to my Bisq BSQ wallet.

The amount of the compensation request is determined by how much value that work has added to Bisq. Additional parameters such as an hourly market rate can also be taken into account in determining the amount, but the important point is that the work has to be complete and useful. The contributors are encouraged to break down their work into smaller chunks that can be finished within a month. It is the result that counts, not the process.

It is important to clarify that as of this moment the Bisq DAO has not been launched yet. Any revenue generated from Bisq trades goes to the arbitrators while the contributors are not being paid yet. They can still submit compensation requests for the work they have done, and the amount of their compensation is tracked on a spreadsheet. They will be paid the earned BSQ amount upon the DAO launch. On average, 50,000 new BSQ is issued every month since October 2017.

#### Uncoloring BSQ Tokens
While new BSQ is created via the genesis transaction and issuance transactions, it can be burned or uncolored in several ways. These include various fees such as trading and voting fees and burned bonds (see below). The uncolored BSQ turns back into BTC which is used as miners' fees. 

### BSQ Supply
There will be an initial supply of 2.5M BSQ from the genesis transaction. The subsequent supply will depend on the amount of compensation requests and the usage of BSQ in the form of trading fees. The compensation requests will increase the BSQ supply while the trading fees will lead to its decrease. Currently, around 50,000 new BSQ is created and nominally distributed to about 14 contributors every month since the end of 2017.

### Trading Fees
In the future, users will be able to buy BSQ tokens and use them as trading fees which will be heavily discounted compared to current trading fees in BTC. Instead of being directly distributed among the contributors, the trading fees will be uncolored which will lead to the decrease in the total BSQ supply. This means that each BSQ will gain in value which is highly beneficial for all stakeholders.

### Stakeholders
Anyone who holds BSQ tokens is considered a stakeholder. As of this moment, the only way to obtain the tokens is by being a contributor. Thus, those who have contributed most to Bisq have the proportionate amount of the BSQ tokens. 

The stakeholders are incentivized to maintain Bisq and to participate in its governance to ensure the success of the project. They have the power to decide how many new tokens are issued every month by voting on compensation requests. They also decide if a project should be prioritized or discarded, to increase or decrease various fees, etc.

### Voting
Once a contributor submits their compensation request, any stakeholder can vote on that request. This includes the contributor submitting the request if they hold any BSQ. The voting weight for each stakeholder is determined by the amount of BSQ stake used in the voting period. You can either upvote, downvote or place a neutral vote for that request. The stakeholders can vote not only on compensation requests but also on other proposals auch as reimbursement requests or proposals to add or remove an asset on the exchange. The stakeholders are encouraged to take voting seriously and need to pay a small voting fee in BSQ which gets uncolored. 

### Bonding
Some high stake roles such as Bisq maintainers, seed node operators or price node operators, require a bond in BSQ for the period of exercising that role. This is done as an insurance against any rogue behavior from those role holders. In the event of defection, that bond is burned, i.e., that BSQ amount is uncolored. This decreases the total supply of BSQ which is beneficial for all stakeholders. This should happen rarely and should not significantly affect the BSQ supply. 

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/).

## Join us!
