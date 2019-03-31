# Bisq P2P network

![bisq_network_visualisation](https://user-images.githubusercontent.com/43150241/55291361-5e7a8680-53cd-11e9-8609-afc5965ff1ba.jpg)
Image from https://github.com/Wimking1987

## Introduction
The Bisq network consists of nodes running the Bisq software, and is a second layer running on top of the Bitcoin network. Just like [the Bitcoin network](btcnetwork.md), it is a peer-to-peer (P2P) network that does not have a central server and is instead made up of individual peers. Bitcoin transactions on Bisq are validated by a handful of Bitcoin full nodes run by trusted contributors, but users are free to connect their own full node to Bisq as well. Upon starting, the Bisq app connects to these nodes. If there is a local Bitcoin full node, the software automatically detects it and connects to it instead.  

## Bisq software
In order to join the network, you need to [download the Bisq software](https://bisq.network/downloads/).
- It is free/open-source software (FOSS) that enables you to trade bitcoin for fiat currencies and cryptocurrencies.
- The software has internal BTC and BSQ wallets as well as pricing data for bitcoin and other currencies.
- It allows you to participate in the Bisq DAO in a self-contained way (make proposals, vote, etc). 
- You can learn more about the software in [the Bisq software doc](bisqsoftware.md).

## Seed nodes
- Every time the Bisq software gets started, it gets connected to seed nodes.
- Seed nodes run the Bisq software, and they introduce users to other Bisq nodes.

## Price nodes
- Price nodes fetch data on cryptocurrency prices and serve it to Bisq nodes. 
- Currently, the price nodes fetch the BTC price in fiat from bitcoinaverage.com, and altcoin data from poloniex.com and coinmarketcap.com.

## Bisq BSQ explorer
[The Bisq BSQ Explorer](https://explorer.bisq.network/index.html) is a Bitcoin full node as well as a Bisq node with a web interface around it. It provides basic info on BSQ transactions.
