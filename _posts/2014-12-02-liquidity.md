---
layout: post
title: What really is liquidity?
---

Bitcoin is known for its high volatility. It is seen as one of the major hinderances which prevents more widespread adoption as medium of exchange [[1]](http://www.coindesk.com/saxo-ceo-bitcoins-liquidity-problems-are-driving-banks-away/). A large number of startups and companies suggested solutions or are actively working on products which aim to reduce this volatility. 

For example, some wallet providers like Coinapult or Bitreserve provide to "lock" in your Bitcoin, effectively selling or hedging them, in order to guarantee a stable dollar wallet value. This is definitely an effective way for consumers to not have to worry about the price volatility. However, why is Bitcoin so volatile in the first place? 

We believe it is because of the lack of liquidity on exchanges, after all the price of Bitcoin is determined on exchanges not on the blockchain. Clearly, exchanges also noticed this and are in a fierce battle for market share (by volume), as their income is mostly dependent on their trading volume. To make their exchange more attractive some offer better commissions to high volume traders, or provide features such as futures and margin trading. Some advertise themselve as "highly liquid" exchanges. However liquidity is never properly defined, at least in the Bitcoin economy. Liquidity is not money on the orderbook and also not volume traded. It is more subtle than that and in this post we will try to make this more accessible and describe the common properties of liquidity.

## Defining Liquidity

Defining and measuring liquidity is not straightforward as it can't be summarised in one number or measure. Also liquidity is not a concept that is either present ("we are highly liquid") or not but rather changes continuously. We attempt to define liquidity as follows

 > Liquidity is the quality of the executions received when trading for a period of time on a market place.

The properties of liquidity usually consist of the following 

- *Trading time*: the ability to execute immediately at a given price. The number of trades per time unit or the inter-trade time is a measure of trading time.

- *Tightness*: the ability to buy and sell at about the same price. The spread and evolution of spread through time is the defining factor of tightness. The spread is also a direct measure of the cost of an immediate market order.

- *Depth*: the ability to buy or sell a certain amount without affecting the current price. The sum of all orders at a given level of the orderbook make up the depth at that given price.

- *Resilience*: the ability to buy or sell a certain amount with minimal influence on the current price. A resilient orderbook is one which reverts back to its previous state after a large order traded through a couple of levels of the orderbook. 

For each of the properties above there's a number of measures you can calculate to assess that particular aspect of liqudity. Some look at orderbook snapshots in time, others look at the evolution of the orderbook through time. Even without measuring the points above are quite intuitive, for example an orderbook with a million dollar on the first level of bid and ask but with only 2 trades a day is clearly not liquid. Liquidity requires a reasonable combination of the above points. Interesting to note here is that we did not mention volume -- usually the prevalent definition of liquidity.

Usually sites like [bitcoinwisdom](http://bitcoinwisdom) or [cryptowatch](http://www.cryptowat.ch) give a good snapshot overview over the state of the orderbooks on various Bitcoin exchanges. 

<p><center>
<img src="/public/ob_static.png" alt="Static Orderbook" align="center" width="30%"></img>
</center>
</p>

For example in the image above we see such a snapshot which shows the spread, depth, and cummulative volume on the book (which could hint towards resilience) at this current moment. 

We could go into a lot of detail what measures are useful, perhaps we will do that in a future post if there's interest, but for now we want to demonstrate the usual lack of liquidity by most measures on Bitcoin exchanges and its effect on the price during a particularly volatile period in November. What we want to demonstrate with this example is that the lack of liquidity leads to highly volatile prices, as individual traders are able to move the market with a few number of large trades due to e.g. a lack of the depth and resilience requirement.

## Lack of Liquidity

The next graph shows the BTCCNY price on OkCoin China in the first three days of December, with the cummulative order flow (running sum of all market order trades) overlaid on the second y-axis. What is immediately visible is the very high correlation between the two series. This is typical for markets with mostly profit-seeking players, where traders follow other traders and as a result the market impact of trades largely agrees with the price. 

<p><center>
<img src="/public/priceflow.png" alt="Price and flow" align="center" width="80%"></img>
</center>
</p>

This also leads to very reactive and volatile markets where large trades are not digested well (i.e. lack of resilience), which is visible in the sharp drop in the morning of the 3 December. Let's have a closer look at the market orders that morning.

<p><center>
<img src="/public/marketorders.png" alt="Market orders" align="center" width="80%"></img>
</center>
</p>

Up until 8:45 it is quiet until one sell trade of slightly more than 200 BTC is executed. From that point on volatility increases a lot and the price drops. If the trader of the first trade would like to sell another 200 BTC 10 minutes later he would get a price that is 2-3% worse than the initial price, directly violating one of the properties of liquidity.

## Solutions

There's no immediate solution to the illiquidity and volatility of Bitcoin markets apart from the overall maturing of the ecosystem. It requires traders with different motivations than just immediate profit-seeking. Our contribution to this is market making




