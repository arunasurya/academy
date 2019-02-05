# An overview of the Bisq ecosystem

## Introduction
In this post, I will give you a general overview of the Bisq ecosystem. At the center of the Bisq ecosystem is the Bisq app, an open-source software that enables you to trade bitcoin for fiat currencies and cryptocurrencies. 

## Bisq peer-to-peer (P2P) Network
The Bisq P2P network consists of nodes running the Bisq software. 
Just like the Bitcoin network, the Bisq P2P network does not have a central server but is instead made up of individual peers.

Some of the Bisq nodes may also be full Bitcoin nodes. There are public Bitcoin nodes run by the Bisq community that are available to the Bisq peers. Upon starting the Bisq app, it connects either to a local Bitcoin full node or several public nodes. In addition to Bisq nodes, the network includes several other nodes, each with a specific function.

### Seed nodes
- Every time the Bisq app gets started, it gets connected to seed nodes.
- Seed nodes run the Bisq software, and they introduce users to other Bisq nodes.

### Price nodes
- Price nodes fetch data from a single centralized website (currently bitcoinaverage.com) and serve it to Bisq nodes.

### Bisq BSQ explorer
[The Bisq BSQ Explorer](https://explorer.bisq.network/index.html) is a Bitcoin full node as well as a Bisq node with a web interface around it. It provides basic info on BSQ transactions.

TODO: add a schematic

## Bisq App
In order to join the Bisq network, you need to [download the Bisq app](https://bisq.network/downloads/). It has internal BTC and BSQ wallets as well as pricing data for bitcoin and other currencies. It allows you to participate in the Bisq DAO in a self-contained way (make proposals, vote, etc). 

## Bisq Participants: 
The Bisq app is maintained by a number of people who are called contributors. Anyone can become a contributor, as long as they provide valuable work for Bisq. 
Users: traders
Contributors (including stakeholders)

Discuss the transfer of value from the users to contributors. 

Introduce Bisq DAO

## More information on Bisq
You can learn more about the app on [the Bisq website](https://docs.bisq.network/getting-started.html).
