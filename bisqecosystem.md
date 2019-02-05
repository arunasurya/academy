# An overview of the Bisq ecosystem

## Introduction
If you are into cryptocurrencies, you may have heard of or even used Bisq, a decentralized exchange that enables you to trade bitcoin for fiat currencies and cryptocurrencies. Although Bisq is an open-source software, it is continuously maintained by a team of dedicated people called contributors. Together with the app, the traders and contributors make up the Bisq ecosystem. In this post, I will provide a brief overview of the Bisq ecosystem, starting with its core, the Bisq app.

## Bisq App
Unlike other cryptocurrency exchanges, Bisq is fully decentralized, meaning that the data is not stored on a central server. If you want to trade, all you need to do is to download and install [the Bisq app](https://bisq.network/downloads/) on your computer, and you become part of the Bisq network. Since all your data is stored locally on your computer, Bisq has no access to your personal data. You need to share specific information only with your trading partner. There is no need for registration or approval from central authority.

The app has internal BTC and BSQ wallets as well as pricing data for bitcoin and other currencies. In addition, it contains the script that specifies rules for governance of the whole project, which will be briefly mentioned later. 

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
The main participants in the Bisq ecosystem are users and contributors. A trader is anyone who trades on Bisq. A contributor is anyone who provides valuable work for Bisq. One can become a contributor by choosing a role from a list of specific roles (e.g. maintainers, operators, ambassadors, etc) or creating their own role.

## Bisq DAO
The Bisq app allows you to participate in the Bisq DAO in a self-contained way.
TODO: Discuss the transfer of value from the users to contributors. Briefly mention BSQ token.

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/)
