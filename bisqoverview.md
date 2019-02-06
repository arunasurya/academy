# An overview of Bisq

## Introduction
If you are into cryptocurrencies, you may be interested in Bisq, a decentralized exchange that enables you to trade bitcoin for fiat currencies and other cryptocurrencies. In this post, I will give you an overview of Bisq, including the Bisq app, the Bisq network and its participants. I will also talk about the unique way Bisq handles its governance and how it algns incentives of its users with those of the contributors.   

## Bisq App
Bisq is decentralized, meaning that the exchange data such as the order book is not stored on a central server. If you want to trade, it is easy to download and install [the Bisq app](https://bisq.network/downloads/) on your computer. The Bisq app is free/open-source software (FOSS) which is maintained and improved by a group of contributors. By running the app, your computer becomes part of the Bisq network. There is no need for registration or approval from any central authorities, you just download and start the app. The app contains an internal BTC wallet.

There are many different payment methods that you can use on Bisq. For instance, if you are using MoneyGram to receive USD in exchange for BTC, you need to add information about your MoneyGram account so that your trading partner can send you USD. Bisq does not automatically send the USD from your trading partner to you, it just gives them the information they need to send USD to your MoneyGram account. Since your data is stored locally on your computer, the rest of the network doesn't know the details about your MoneyGram account.

TODO: add stats on Bisq (how long it has been running, # of users, etc)

## Bisq Network
The Bisq network consists of nodes running the Bisq software. Just like the Bitcoin network, it is a peer-to-peer (P2P) network that does not have a central server and is instead made up of individual peers. Some of the Bisq nodes may also be full Bitcoin nodes, typically running the Bitcoin Core software. There are public Bitcoin nodes that are run by some contributors. Upon starting, the Bisq app connects to these nodes. If there is a local Bitcoin full node, the Bisq app automatically detects it and connects to it instead. In addition to Bisq nodes, the network includes several other nodes, each with a specific function.

### Seed Nodes
Every time the Bisq app gets started, it gets connected to seed nodes. Seed nodes run the Bisq software, and they introduce users to other Bisq nodes. 

### Price Nodes
Price nodes fetch data on cryptocurrency prices and serve it to Bisq nodes. Currently, the price nodes fetch this data from a single centralized website, bitcoinaverage.com.

## Bisq Participants
The main participants in Bisq are users, arbitrators and contributors. A user is anyone who trades on Bisq. An arbitrator is a person who solves any trading disputes between trading partners. A contributor is anyone who provides valuable work for Bisq. You can become a contributor by doing some important work and then filing for a compensation request. You can choose a specific role from a list of [roles](https://docs.bisq.network/roles.html) such as maintainers, operators and administrators. You are also free to define your own role that suits your background and strengths. You decide your own working schedule, the amount of work you want to do in a given period and how frequently you want to contribute. Some pre-defined roles require consistent contributions while others are more flexible.

At this point, you may wonder if the contributors and arbitrators ever get paid for their work. They do. This brings us to the Bisq DAO.

## Bisq DAO
It is clear that the users benefit from Bisq by being able to trade in a secure way without compromising their privacy. In order to continue maintaining and improving Bisq in a sustainable way, the contributors need to get paid for their work. The Bisq DAO (Decentralized Autonomous Organization) is an effective way to transfer value from Bisq users to its contributors. 

### Compensation Requests
At the end of each month, a contributor files a compensation request for the work they have done in the previous month. The amount requested is determined by how much value that work has added to Bisq. Additional parameters such as an hourly market rate can also be taken into account in determining the amount, but the important point is that the work has to be complete and useful. The contributors are encouraged to break down their work into smaller chunks that can be finished within a month.

It is important to clarify that as of this moment the Bisq DAO has not been launched yet. Any revenue generated from Bisq trades goes to the arbitrators while the contributors are not being paid yet. They can still submit compensation requests for the work they have done, and the amount of their compensation is tracked on a spreadsheet. They will be paid that amount upon the DAO launch. You may wonder, what exactly will the contributors be paid in? Upon DAO, Bisq will issue its own colored coin basedon on the Bitcoin blockchain, the BSQ token, which will be used to reward the contributors and in Bisq governance in general. 

### Stakeholders
Anyone who holds BSQ tokens is considered a stakeholder. As of this moment, the only way to obtain the tokens is by being a contributor. Thus, those who have contributed most to Bisq have the proportionate amount of the BSQ tokens. In the future, users will be able to buy BSQ tokens and use them as trading fees which will be heavily discounted compared to trading fees in BTC. 

### Voting
Once a contributor submits their compensation request, any stakeholder can vote on that request. This includes the contributor submitting the request if they hold any BSQ. The voting weight for each stakeholder is determined by the amount of BSQ stake used in the voting period. You can either upvode, downvote or have a neutral vote. The stakeholders can vote not only on compensation requests but on any other proposal. 

## BSQ Token
The BSQ token is a colored coin based on the Bitcoin blockchain. The Bisq app contains the script for issuing and burning the tokens. There are two ways the BSQ tokens can be issued, through the genesis transaction and through decentralized issuance.

### Genesis Transaction
Upon the Bisq DAO, Bisq developers create a bitcoin transaction and label it in the Bisq source codeas the 2.5BTC (that was donated) will be used to create 2.5M BSQ. Since there are 100M satoshis in 1BTC, each BSQ is equal to 100 satoshis. This 2.5M BSQ will be distributed to past contributors. 

### Decentralized Issuance
Any contributor can issue new BSQ by filing for a compensation request at the end of each month. For instance, I file a request for 1000BSQ. Since  

### Burning

In addition to the BTC wallet, the Bisq app also has a BSQ wallet.


The stakeholders are incentivized to maintain Bisq and to participate in its governance to ensure that the project continues to be successful. They have the power to decide how many new tokens are issued every month by voting on compensation requests. They also decide if a project should be prioritized or discarded, to increase or decrease various fees, etc.  

Apart from all the great things that the Bisq app has, it also allows you to participate in the Bisq DAO in a self-contained way.
 

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/).

## Join us!
