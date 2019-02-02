# Bisq P2P network

## Core concepts
- Bisq app
- Seed nodes
- Price nodes
- Bisq BSQ explorer

## Introduction
The Bisq P2P network consists of nodes running the Bisq software. 
Just like [the Bitcoin network](btcnetwork.md), the Bisq P2P network does not have a central server but is instead made up of individual peers.

In addition to being Bisq nodes, some of them may also be full Bitcoin nodes. 
There are public Bitcoin nodes (run by the Bisq community) that are available to the Bisq peers. 
When the users start the Bisq app, it connects either to a local Bitcoin full node or several public nodes. 

## Bisq app
In order to join the network, you need to [download the Bisq app](https://bisq.network/downloads/).
- Bisq is an open-source software that enables you to trade bitcoin for fiat currencies and cryptocurrencies.
- It has internal BTC and BSQ wallets as well as pricing data for bitcoin and other currencies.
- It allows you to participate in the Bisq DAO in a self-contained way (make proposals, vote, etc). 
- You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).

## Seed nodes
- Every time the Bisq app gets started, it gets connected to seed nodes.
- Seed nodes run the Bisq software, and they introduce you to other Bisq nodes.

## Price nodes
- Price nodes fetch data from a single centralized website (currently bitcoinaverage.com) and serve it to Bisq nodes.

## Bisq BSQ explorer
[The Bisq BSQ Explorer](https://explorer.bisq.network/index.html) is a Bitcoin full node as well as a Bisq node with a web interface around it.
- it provides basic info on BSQ transactions.
