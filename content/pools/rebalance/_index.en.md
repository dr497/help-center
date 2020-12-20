---
title: "How do pools rebalance?"
date: 2020-12-20T11:02:05+06:00
lastmod: 2020-12-20T11:02:05+06:00
weight: 1
draft: false
# search related keywords
keywords: ["pool", "rebalance"]
---

# First Rebalance i.e Initaliziation

Let's take the Ecosystem Pool as an example. Until December 22nd only USDC can be deposited in the pool, so let's say that on December 22nd just before it's initaliziation, people deposited 100,000 USDC in the pool. The breakdown of the pool would be as follow:

| Coin | Size    | Spot price |
| ---- | ------- | ---------- |
| FIDA | 0       | \$0.1      |
| SRM  | 0       | \$1.2      |
| SOL  | 0       | \$1.6      |
| LQID | 0       | \$0.2      |
| USDC | 100,000 | \$1        |

Before it's initaliziation the pool contains USD$ 100,000 so it needs to buy $ 100,000/4 = \$ 25,000 worth of each token, so after it's initaliziation the pool will be as follow:

| Coin | Size     | Spot price |
| ---- | -------- | ---------- |
| FIDA | 250,000  | \$0.1      |
| SRM  | 20,833.3 | \$1.2      |
| SOL  | 15,625   | \$1.6      |
| LQID | 125,000  | \$0.2      |
| USDC | 0        | \$1        |

# Weekly Rebalance

Let's keep the previous example, let's assume that the spot prices have changed to the following:

| Coin | Size     | Spot price | USD worth |
| ---- | -------- | ---------- | --------- |
| FIDA | 250,000  | \$0.2      | 50,000    |
| SRM  | 20,833.3 | \$1.1      | 22,916.63 |
| SOL  | 15,625   | \$1.8      | 28,125    |
| LQID | 125,000  | \$0.25     | 31,250    |

The pool is now worth \$132,291.63 and will need to rebalance to allocate \$ 132,291.63 / 4 = \$ 33,072.9 in each asset. So the pool will have to sell some of it's FIDA to buy SRM, SOL and LQID. The pool will buy from the orderbook at the best average entry price. After the rebalance the pool will look like:

| Coin | Size      | Spot price | USD worth |
| ---- | --------- | ---------- | --------- |
| FIDA | 165,364.5 | \$0.2      | 33,072.9  |
| SRM  | 30,066.27 | \$1.1      | 33,072.9  |
| SOL  | 18,373.83 | \$1.8      | 33,072.9  |
| LQID | 132,291.6 | \$0.25     | 33,072.9  |
