# An overview of the Bisq Network

## Introduction
If you are into cryptocurrencies, you may be interested in Bisq, a decentralized exchange that enables you to trade bitcoin for fiat currencies and other cryptocurrencies. In this post, I will give you an overview of the Bisq network.   

## Bisq Software
Bisq is decentralized, meaning that the exchange data such as the order book is not stored on a central server. If you want to trade, it is easy to download and install [the Bisq app](https://bisq.network/downloads/) on your computer. The Bisq app is free/open-source software (FOSS) which is maintained and improved by a group of contributors. By running the app, your computer becomes part of the Bisq network. There is no need for registration or approval from any central authorities, you just download and start the software. It contains an internal BTC wallet.

Since its launch in April 2016, Bisq has been providing free exchange services without any major issues, with the median monthly growth in trades of 50%. It has processed about 22,000+ trades, and has been generating revenue.

There are many different payment methods that you can use on Bisq. For instance, if you are using MoneyGram to receive USD in exchange for BTC, you need to add information about your MoneyGram account so that your trading partner can send you USD. Bisq does not automatically send the USD from your trading partner to you, it just gives them the information they need to send USD to your MoneyGram account. Since your data is stored locally on your computer, the rest of the network doesn't know the details about your MoneyGram account.

## Bisq Network
The Bisq network consists of nodes running the Bisq software. Just like the Bitcoin network, it is a peer-to-peer (P2P) network that does not have a central server and is instead made up of individual peers. Some of the users running Bisq nodes may also run full Bitcoin nodes, typically the Bitcoin Core software. There are public Bitcoin nodes that are run by some contributors. Upon starting, the Bisq app connects to these nodes. If there is a local Bitcoin full node, the Bisq app automatically detects it and connects to it instead. 

In addition to Bisq nodes, the network includes several other nodes, each with a specific function. Every time the Bisq app gets started, it gets connected to seed nodes. Seed nodes run the Bisq software, and they introduce users to other Bisq nodes. Price nodes fetch data on cryptocurrency prices and serve it to Bisq nodes. Currently, the price nodes fetch the BTC price in fiat from bitcoinaverage.com, and altcoin data from poloniex.com and coinmarketcap.com.

## More information on Bisq
You can learn more about the Bisq software on [the Bisq website](https://docs.bisq.network/getting-started.html).
For more technical details of the Bisq P2P network, please visit [this blog post by Manfred Karrer](https://bisq.network/blog/new-p2p-network/).

