---
layout: post
title: "Trading Plan"
date: 2012-04-29 01:45
comments: false
categories: ['forex', 'trading']
---

This post describes my trading plan. It is good that this is a semi-public (semi-public in that I don't actively advertise this site, people who come here will only come here by accident) forum. It is good because it will force me to write a good trading plan and hopefully will make me follow it.

<!-- more -->

## Beliefs
* I believe I only need to master one setup to be a consistently profitable trader. After I have mastered one setup and "own it" I can start to master another setup ... ad infinitum.

* I believe that Price Action trading is the best approach to market analysis, because most technical analysis indicators are derivatives of price so why not just use price.

* I believe that trading is gambling but it is possible to fix the odds slightly in your favour.

* I don't care what moves the Forex market, my approach is very short term. So macro economic analysis will have no impact on my trading.

* I do need to be conscious of calendar events while I have a trade open.

* I believe that the psychological aspect (discipline, control of fear and greed) of trading is the most important thing in trading.

* I believe the second most important thing is money management.

* I believe the technical aspects of trading are irrelevant if you don't have good money management and control of your mind.

* I do not know what the market will do. All I can do is use my experience and skills to allocate a probability to what the market will do.

* I believe that compounding is vital.

* I believe I can be successful at trading only if I take control of my self discipline and mind.

* I believe losses are part and parcel of trading. Therefore losses should not upset me. Taking losses does not mean I'm a loser.

* I believe leverage is a two edged sword, that holds the potential to bring me down.

## Objectives

### Annual
* Achieve an average 200% increase in Trading Capital
* Measurable (what?) performance improvement in mastering strategies.
* Develop profitable trading strategy or strategies using R
* Low risk, high probability

### Monthly
* Achieve an average 16% increase in Trading Capital
* Remain consistently profitable
* Trading Plan refinement
* Strategy refinement

### Weekly
* Achieve an average 4% increase in Trading Capital
* Maintain strict compliance with trading business plan
* Consistent discipline and execution performance
* Review and refine trade set-ups
* Define weekly revenue/profit targets

### Daily
* Execution refinement
* Discipline refinement
* Journal entry refinement

## Self Assessment

### Why
* I want to be a trader it offers an income which I will be unable to achieve elsewhere.
* I want to be a trader because it suits my personality and character
* I want to be a trader because I can enjoy the freedom of being able to trade from anywhere in the world.
* I believe  I can achieve my objectives because I have learned a lot from my previous trading experience. 

### Weakness
* I lack self discipline
* I do not have control of my emotions.

### Strengths
* TODO
	
## Markets
I have chosen to trade Forex. I have a couple of years experience trading equities in the USA via Contracts for Difference (CFD) But for the size of the account, I was trading, the round trip expenses were too much. So this time around I wanted a  market where I did not have to pay any transation fees on top of the spread. No transaction fees and great leverage are the reasons I chose Foreign Exchange as my preferred market to trade.

## Instruments
My main criteria for an appropriate instrument was one with a low spread and high liquidity. Most crosses have a fairly high spread making them ineligible. Any of the major's were going to be OK, so pretty much randomly I chose the AUDUSD, EURUSD, and GBPUSD. But will focus for at least 12 months on the AUDUSD.

## Broker
I have two brokers [FXPro][001] and [Pepperstone][002]. When I was hunting for a broker, my major criteria was to find a broker that had tight spreads. These two brokers should allow me to trade AUDUSD, EURUSD and GBPUSD with a 1 pip spread.

I have only funded FXPro at this stage, and plan to use Pepperstone as a backup. FXPro has a slight pecularity in that there are two types of accounts, one type uses the [Market Maker][006] model and the other uses an [ECN][005] model. I have opened an account of each type but only funded the Market Maker model account. The main difference between the two accounts are that the ECN account offers a more direct route to the interbank market, it is aimed a bigger players and commissions are charged per transaction.


## Platform
A platforms is required for strategy development, indicator development, charting and execution. I will use [R][003] for strategy development and [MT4][004] for indicator development.

Financial considerations and a desire to keep my monthly costs down for at least 12 months precludes the option of getting a seperate data and charting package. Therefore I will utilise the broker supplied platforms for charting and execution. Currently both Pepperstone and FXPro offer [MT4][004] for their charting and execution platforms.

## Workflow

### PreMarket
TODO

### InMarket
TODO

### PostMarket
TODO

## Timeframes
I'm trading a small account. Therefore to maximise the magic of compounding, I'm will trade short-term on a M15 timeframe. I do not believe I have the temperament or quickness of mind for shorter timeframes.

## Trading Hours
Trading takes intense concentration, therefore I dont' believe I can be effective for an entire trading day. So I need to trade just a subset. There are two particular time periods that have high liquid and volatility which are the conditions best suited to create an environment in which it is possible to make some pips. The two periods are the first 3 hours of the London Open which is 0800-1100 UTC and the intersection of the London Open and the New York Open which is from 1300-1600 UTC. I will choose to trade one of these periods each day.

## Trading Limits
* Allowed positions per day : 1
	
## Stop Trading Signals
* 6% Rule
* Outside Defined Trading Hours
* Reached Daily Loss Limit
* Reached Week Loss Limit
* Reached Month Loss Limit	
* Emotional Drained : Tired, Depressed, Angry, Exuberant, Invincibiliy
* Distracted, UnableToConcentrate, UnableToFocus
* When Feel Impulse to trade Hunch, Bias or outside of plan
* Volume is consistently low
* Usual setups not working
* Frequent Trend Change (Chop)

## Journal
I will journal all my trades on the heterodoxic.com blog under the category Execution. I will also undertake to complete a daily analysis each day prior to the London open at 0800 UTC. I have setup two Octopress templates that set out the structure and content of these journal entries. TODO

## Log
I will log all my trades using journal.xlsx. This journal calculates position size, risk reward, risk.multiple which I will complete before executing a trade.

## Portfolio
TODO

## Risk Management

{% blockquote %}
equity = acctbal + open(win) - open(lose)
{% endblockquote %}

### Capital Preservation
* MaxTrade		: 5% equity
* MaxAll		: 25% equity
* MaxDailyLoss	: 5% equity
* MaxWeekLoss 	: 10% equity
* MaxMonthLoss	: 20% equity
* Never average down.
* Miniumum R:R 2:1
* Cut Losses
* AdjustStops to protect 80% of profit
* Never allow WinningTrade to become a LosingTrade

I should be risking an absolute maximum of 2% of my equity on a trade. But my account is so miniscule that I feel it is necessary to risk 5%.

Maximum leverage 100:1, again, way too much, I should only be applying a maximum of 50:1. But the miniscule account problem rears its ugly head.

If my account does grow then I will institute sane money management rules, 2% of equity and 50:1 leverage.

## Discipline
### Withdrawals
This area is important because one thing I found when trading previously was, if you leave money in your account you will blow it.

Money earned from the markets is considered by some to be just a temporary loan, as the market will take it back. The trading analogy to a casino is strongly correlated.

Each time my account increases by AUD1000 I will withdraw that AUD1000. This has the beneficial side effect of giving a reward for doing well.

### Funding
TODO

### WindfallProfits
TODO

### DisastrousLosses
TODO

### ConsecutiveLosses
TODO

### Rewards
TODO

### Punishment
* MaxTradesPerDay 				: StopTrade(period = "7")
* Outside Defined Trading Hours : StopTrade(period = "7")

## Resources
This is only a subset of my forex resources, most trading including forex resources are on my hard drive and in my chrome bookmarks.

### Web
* [Steve Hopwood][023]
* [Mataf][007]
* [BabyPips][020]

### Mentor
In the sense that these people are people whose opinion and methodology I respect and agree with.

* [Trading Naked][019]
* [Nial Fuller][011]
* [Crossing Wall Street][012]
* [James Sixteen][008]
* The London Group
* [Brian Shannon][013]
* [Stockbee][018]
* [Joe Fahmy][014]
* [Dave Landry][015]
* [Peter Brandt][016]
* [Pascal Willain][017]

### Tools
* [FXPro][001]
* [Pepperstone][002]
* [Economic Calendar][022]
* [Octopress][009]
* [MT4][004]
* [R][003]
* [SnagIT][010]


## Strategies
A Trading strategies, trading setups, and trading systems are synonyms, they describe a set of rules for executing a trade. A strategy can lie somewhere on a continumn between 100% discretionary and 100% mechanical. Whether you prefer a discretionary or mechanical approach is something you will struggle with and eventually find the right mix.

Economic calendar events will have their own strategy section. As they are strategies. (Define strategy for specific cal. events eg. FOMC(NoTrade), OptionExpiry(NoTrade))


The strategies I utilise are:

* [Alina][021]
* [Ekterina][024]

## Appendix

### Naming Conventions
MT4 Profiles are named according to PAIR-STRATEGYNAME. MT4 Templates are named by PAIR-TIMEFRAME-STRATEGYNAME. All timeframes use minutes so 4 Hour Timeframe is 0240 minutes or Daily timeframe is 1440 minutes etc etc. All our strategies can be found on the blog so we can always backtrack to the strategy to get naming information. For example I might see a profile called AUDUSD-ALINA or a template called AUDUSD-M1440-ALINA but its been a while so I forget what ALINA is/does, so I can just refresh my memory on the blog.


[001]:http://www.fxpro.com.au
[002]:http://www.pepperstone.com.au
[003]:http://www.r-project.org/
[004]:http://www.metaquotes.net/
[005]:http://fxpro.com.au/trading/cfd/ecn
[006]:http://fxpro.com.au/trading/cfd/mt4
[007]:http://www.forexticket.biz/#en
[008]:http://www.james16group.us/
[009]:http://www.octopress.net
[010]:http://www.snagit.com
[011]:http://www.learntotradethemarket.com/
[012]:http://www.amazon.com/Crossing-Wall-Street-Independent-Financial/dp/0615510132
[013]:http://www.alphatrends.net
[014]:http://www.joefahmy.com
[015]:http://www.davelandry.com
[016]:http://www.peterlbrandt.com
[017]:http://www.effectivevolume.com
[018]:http://www.stockbee.biz
[019]:http://www.trading-naked.com
[020]:http://www.babypips.com/
[021]:http://heterodoxic.com/blog/2012/04/29/strategy-alina/
[022]:http://www.babypips.com/tools/forex-calendar/
[023]:http://www.stevehopwoodforex.com
[024]:http://heterodoxic.com/blog/2012/04/29/strategy-ekterina/
