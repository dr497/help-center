---
title: "市价订单"
date: 2020-11-26T11:02:05+06:00
lastmod: 2020-11-26T11:02:05+06:00
weight: 4
draft: false
# search related keywords
keywords: ["市价", "订单", "下单"]
---

我们来假设一下，假如您需要立即执行一笔交易，并又不想等待太久才完成成交。Bonfida是目前是唯一一个可以提供市价订单的Serum前端接口。
事实上，市价订单仅仅是把您想要执行的交易扔到订单薄中，根据现有的市场流动性来完成交易。您不需要等待订单完成，可以把它看做是一个Swap，只不过需要留意可能会发生的潜在滑点。

![market-buy](market-buy.png)
