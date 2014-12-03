---
layout: post
title: What really is liquidity?
comments: True
---

Bitcoin is known for its high volatility. It is seen as one of the major hinderances which prevents more widespread adoption as medium of exchange. Consequently, a large number of industry professionals are working on solutions which aim to reduce the impact of volatility. 

For example, some wallet providers like Coinapult or Bitreserve allow to "lock in" your bitcoin, similar to hedging with forward contracts, in order to guarantee a stable US dollar equivalent value. This can be an effective way for consumers to alleviate the effects of price volatility. However, why is bitcoin so volatile in the first place?

We believe one major reason is the lack of liquidity on exchanges. After all, the price of bitcoin is determined on exchanges and not on the block chain. Most exchanges also noticed this and are in a fierce battle for market share, as their income partly depends on users' trading volume. To make their exchange more attractive some offer better commissions to high volume traders, or provide features such as futures and margin trading. Some exchanges advertise themselves as "highly liquid", however, how is that liquidity actually defined? Liquidity is not simply  money on the order book or volume traded. It is more subtle than that and in this post we will try to make the concept more accessible.

## Defining liquidity

Defining and measuring liquidity is not straightforward as it cannot be summarised in one number. Liquidity is also not a concept that is either present ("we are highly liquid") or not, but rather changes continuously. We attempt to define liquidity as follows

 > Liquidity is the quality of executions received when trading for a period of time on a market place.

Here, quality of executions refers (but is not limited) to 

- *Trading time*: the ability to execute immediately at a given price. The number of trades per minute or the average inter-trade time is a relevant measure.

- *Tightness*: the ability to buy and sell at about the same price. The difference between bid and ask price, or spread, is the defining factor of tightness. The spread is also a direct measure of the cost of a market order.

- *Depth*: the ability to buy or sell a certain amount at any time. The sum of all limit orders at a given level of the orderbook make up the depth at that price.

- *Resilience*: the ability to buy or sell a certain amount with minimal influence on the current price. A resilient orderbook is one which reverts back to its previous state after a large market order traded through a couple of levels of the orderbook. 

For each of the properties above there is a number of measures one can calculate to assess that particular aspect of liqudity. Some look at orderbook snapshots in time, others look at the evolution of the orderbook over time. Even without measuring the observables above some qualitative conclusions are intuitive: An order book for instance with a million dollar on the first level of bid and ask but with only two trades a day is clearly not liquid. 

Real liquidity requires a reasonable combination of the above characteristics. Note that it might be possible to define liquidity as shown above without even mentioning traded volume -- an often evoked measure of liquidity across the industry. 
To the interested reader, sites like [bitcoinwisdom.com](http://bitcoinwisdom.com) or [cryptowat.ch](http://www.cryptowat.ch) give a good overview over the state of the order books on various bitcoin exchanges. 

<p><center>
<img src="/public/ob_static.png" alt="Static Orderbook" align="center" width="30%"></img>
</center>
</p>

In the figure above we show a snapshot reporting spread, depth, and cumulative volume on the book taken from [cryptowat.ch](http://www.cryptowat.ch). 

We could go into a lot of detail what measures are useful, perhaps we will do that in a future post if there is interest. For now we only want to demonstrate the usual lack of liquidity by most measures on bitcoin exchanges and its effect on the price during a particularly volatile period in December. We show evidence that individual traders are able to move the market with a small number of large trades due to a lack of depth and resilience requirements.

## Lack of liquidity

The next graph shows the BTCCNY price on OKCoin China in the first three days of December overlaid with the cumulative order flow (cumulative sum of all market order transactionss in BTC) on the right hand side vertical axis. Both time series appear highly correlated. This is indicative of rather illiquid markets with mostly profit-seeking players, where large aligned order flows drive the price and vice versa.

<p><center>
<img src="/public/priceflow.png" alt="Price and flow" align="center" width="80%"></img>
</center>
</p>

Low liquidity and reactive trading leads to volatile markets where the impact of large trades is not absorbed well but instead amplified. The sharp price drop in the morning of 3 December provides just one example. 

The following figure takes a closer look at individual market orders that morning.

<p><center>
<img src="/public/marketorders.png" alt="Market orders" align="center" width="80%"></img>
</center>
</p>

Up until 8:45 it is all quiet when one sell trade of slightly more than 200 BTC is executed. From that point on volatility increases a lot and the price drops. If the trader of the first trade wanted to sell another 200 BTC 10 minutes later he would have received a price 2-3% worse than the initial one.

## Possible solutions

There's no immediate solution to the illiquidity and volatility of bitcoin markets apart from a gradual maturing of the ecosystem. However, we believe that market makers like ourselves can play a crucial role in speeding up this process.



