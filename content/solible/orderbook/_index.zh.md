---
title: "Orderbook system"
date: 2020-11-26T11:02:05+06:00
lastmod: 2020-11-26T11:02:05+06:00
weight: 1
draft: false
# search related keywords
keywords: ["orderbook", "solible", "NFT"]
---

Solible is a real time NFT auction house implemented with a trading orderbook system, similar to any exchanges you might use.

![orderbook-1](orderbook-1.png)

As any order book you will have, for each items on sale, from top to bottom:

- Sell orders (e.g 2500)
- Last trade (e.g 900)
- Buy orders (e.g 120)

_With the above example, placing a bid lower than 2,500, it could be considered as an open order ; while placing a bid at 2,500 (or over) as a market buy._

_A seller changing its 2,500 limit sell to 120, would, in this case, result in a buy from the 120 order._
