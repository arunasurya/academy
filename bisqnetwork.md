# An overview of the Bisq network

## Introduction
If you are into cryptocurrencies, you may be interested in Bisq, a decentralized exchange that enables you to trade bitcoin for fiat currencies and other cryptocurrencies. The Bisq app is open-source software which is maintained and improved by a group of contributors. 

## Bisq App
Bisq is decentralized, meaning that the exchange data such as the order book is not stored on a central server. If you want to trade, it is easy to download and install [the Bisq app](https://bisq.network/downloads/) on your computer. By running the Bisq app, your computer becomes part of the Bisq network. There is no need for registration or approval from any central authorities, you just download and start the app. There are many different payment methods that you can use on Bisq. For instance, if you are using MoneyGram to receive USD in exchange for BTC, you need to add information about your MoneyGram account so that your trading partner can send you USD. Bisq does not automatically send the USD from your trading partner to you, it just gives them the information they need to send USD to your MoneyGram account. Since your data is stored locally on your computer, the rest of the network doesn't know the details about your MoneyGram account.  

## Bisq Network
The Bisq network consists of nodes running the Bisq software. Just like the Bitcoin network, it is a P2P network that does not have a central server and is instead made up of individual peers. Some of the Bisq nodes may also be full Bitcoin nodes running the Bitcoin Core software. There are public Bitcoin nodes run by the Bisq community that are available to Bisq peers. Upon starting the Bisq app, it connects either to a local Bitcoin full node or several public nodes. In addition to Bisq nodes, the network includes several other nodes, each with a specific function.

### Seed nodes
Every time the Bisq app gets started, it gets connected to seed nodes. Seed nodes run the Bisq software, and they introduce users to other Bisq nodes. 

### Price nodes
Price nodes fetch data from a single centralized website (currently bitcoinaverage.com) and serve it to Bisq nodes.

### Bisq BSQ explorer
[The Bisq BSQ Explorer](https://explorer.bisq.network/index.html) is a Bitcoin full node as well as a Bisq node with a web interface around it. It provides basic info on BSQ transactions.

TODO: add a schematic

## Bisq Participants
The main participants in the Bisq ecosystem are users and contributors. A user is anyone who trades on Bisq. A contributor is anyone who provides valuable work for Bisq. One can become a contributor by choosing a role from a list of specific roles (e.g. maintainers, operators, ambassadors, etc) or creating their own role. 

What makes Bisq unique among other open-source projects is its special way of transfering value from users to contributors.

## Bisq DAO
The Bisq app allows you to participate in the Bisq DAO in a self-contained way.
TODO: Discuss the transfer of value from the users to contributors. Briefly mention BSQ token.

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/)
