---
layout: post
title: What is driving bitcoin price volatility?
comments: True
---
<div class="message">
This year has seen plenty of speculation on the driving forces behind bitcoin's depreciation. One often cited suspect is increased spending which leads to downside pressure as merchants have to sell off their acquired bitcoin holdings. Here, we outline the interplay between market makers and takers in bitcoin price formation and show how an imbalance can lead to high price volatility.
</div>

## Maker-taker interaction and bitcoin price formation

The volatility of bitcoin prices is often mentioned as one of the obstacles slowing down public adoption. A contributing factor to high volatility is low liquidity. Although <a href="http://blog.queueco.com/2014/12/03/liquidity/">liquidity</a> is a diverse concept as discussed in our previous post, it is characterised by the ability of the market to absorb large buy or sell orders.

The price formation of bitcoin mainly happens on exchanges which bring together buyers and sellers of digital currencies. Traders on exchanges can be categorised into market makers and takers: market makers quote limit orders and signal their willingness to buy or sell bitcoin at two distinct prices, the bid and ask price. They then collect the price difference, or spread, as compensation for not being in control of when their orders are executed. Effectively they take the risk of buying (selling) bitcoin just before the price drops (rises).

Market takers in contrast pay the bid-ask spread in exchange for immediate execution of their market orders. Thus, they remove liquidity from the order book. Merchants who dispose of their bitcoin holdings fall into this category just like most profit-seeking traders.

If there are not enough quotes by market makers on the order book, large market orders will be able to shift the mid price significantly as they eat their way through the sparse limit quotes. This in turn manifests in high levels of volatility and can lead to the huge price swings the industry has become accustomed to.

To stabilise the price of bitcoin in the longer term, it is thus crucial that market makers add liquidity to the order books and help to absorb the price impact of huge market orders.

## An example of how traders drive the bitcoin price

Taking liquidity by executing market orders is favourable if there are structural inefficiencies and mis-pricing. In the following, we provide an illustrative example of how these inefficiencies can be traded and outline why low liquidity can foster volatility.

The first figure below shows the average hourly traded BTC volume of Bitstamp (BTCUSD, UTC timezone, data obtained from [bitcoincharts.com](https://bitcoincharts.com)). Since Bitstamp is one of the most prominent European exchanges that facilitates exchange of bitcoin and USD, the traded volume is largest in the overlapping US morning / European afternoon sessions, while dropping off significantly overnight. 

<p><center>
<img src="/public/hourofday.png" alt="HourlyVolume" align="center" width="80%"></img>
</center>
</p>

Interestingly, we observe heavy activity early in the European morning that does not fit into the general night-day rhythm of activity. Around 7-10am UTC time, consistently increased trading volumes were recorded over the past 5 month period.

Obviously there is a plethora of possible explanations of this phenomenon, however, we suggest the possibility that it might be due to regular merchant activity. 

To illustrate how market takers can benefit from such a periodic pattern we develop a systematic trading strategy that follows the regular flows in the European morning. Our strategy thus benefits from the price impact of large market orders and could even reinforce them. 

Figure 2 displays back-tested cumulative percentage returns of our market taker strategy, which shows strong performance over the previous five months. The fact that the model works can be attributed to the lasting price impact of large market orders and benefits from price volatility.

We believe that increased market making activity can reduce volatility by absorbing the price impact of large orders.

<p><center>
<img src="/public/returns.png" alt="StrategyReturns" align="center" width="80%"></img>
</center>
</p>
