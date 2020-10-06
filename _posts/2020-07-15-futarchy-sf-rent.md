---
title: SF Housing Futarchy Example
show_author: true
comments: true
date: 2020-07-15 02:00:00
---



> Futarchy, in one short post. With one straightforward application.

#### A. The Problem (and Meta-Problems)

The SF housing problem is well-known: absurdly-high rent. (See [here](https://www.sfgate.com/realestate/article/Bad-news-if-you-re-planning-to-save-money-on-rent-14082788.php) or just [look on Apartments.com](https://www.apartments.com/san-francisco-ca/)).

The meta-problem (ie, "why is the rent absurdly high?") is also well-known: lack of supply. (See [here](https://www.trulia.com/research/elasticity-2016/), and compare [SFs little townhomes to NYC's skyscrapers](https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population_density)).

The meta-meta-problem (ie, "why is the housing supply so low?") is also well-known: restrictions on housing construction. (See ["baffling alchemy of [SF]'s rules, its housing culture, and the dispositions of San Franciscans"](https://sf.curbed.com/maps/map-sf-housing-delayed-cancelled-monster-mission-projects)).

And finally, the meta-meta-meta-problem (ie, "Where did these new-housing-restrictions come from any why can't SF get rid of them?") is also well known: renters at a political disadvantage. (See ["unorganized and unorganizable"](https://www.theatlantic.com/ideas/archive/2020/02/building-enough-housing-requires-unlikely-coalition/606739/), ["home value insurance"](https://www.dartmouth.edu/~wfischel/Papers/02-03.pdf) -- and remember that SF has [more renters than owners](https://www.rentcafe.com/blog/rental-market/market-snapshots/decade-housing-trends-methodology/) and is [theoretically](https://www.pdx.edu/prc/sites/www.pdx.edu.prc/files/Who_Votes_for_Mayor_Sept_2015.pdf) [a democracy](https://en.wikipedia.org/wiki/Government_of_San_Francisco)).


But this "unorganized and unorganizable" problem, happens to be one that prediction markets can probably solve! Once the root problem is solved, all the other solutions should fall in line automatically.


How can prediction markets solve political disorganization? 


#### B. Solution

First, identify a **metric of accountability**. In this case: *rent per square foot* (for [example](https://www.apartmentguide.com/blog/cities-with-most-expensive-apartments-per-square-foot/)) in years 2021, 2022, 2023, etc.

Second, identify the **decision variable**. In this case: *voting* [for Mayor, Board of Supervisors, and/or [direct ballot initiatives](https://en.wikipedia.org/wiki/Initiative)].

Then, as always, you make a new market crossing Accountability with Decision:

       ----[Rent ($/ft2) 1BR, 2024 m=$2, M=$10, L]--->
       |          Min   Max
       |    No   0.25  0.25
    [Keep   Yes  0.25  0.25
     Mayor,
     2023?] 
       |
       \/ 

This market destroys political disorganization, merely by existing. It does so because it helps all voters **easily** understand **the connection** between *their vote* and *next year's rent*.

To understand how, we first need to interpret these market prices.

#### C. What does it mean?

This market is divided into four states. At onset, shares of each state is automatically priced at 0.25 $ per share (ie, 25%).

( It is quite possible to build a BTC-exclusive prediction market, that nonetheless generates returns as if it were priced in dollars (and thus, for all intents and purpose, a market that "is" denominated in USD). It is just a little complicated and requires 8 states. See "portfolio replication" in my [Excel LMSR Guide](http://bitcoinhivemind.com/papers/LogMSR_Demo.xlsx). )

The vertical dimension measures the liklihood of the Mayor being re-elected (or of the [Mayor's party](https://en.wikipedia.org/wiki/Mayor_of_San_Francisco#List) remaining in power, or of the ballot initiative passing, or of whatever is put on this axis).

The horizontal dimension measures the average price (in USD per square ft) of a SF 1 Bedroom apartment. It is very important to choose a reliable source for this information, and to define that source very precisely. Also, we need to know *by when* that source will have published its figures (time is not of the essence, but we cannot make use of the figures unless they are eventually published). I also placed bounds on this condition -- a minimum of $2 and a maximum of $10.

In the example above, the market prices are all equal -- (25-25-25-25). The interpretation is therefore:

* The Mayor has a 50% chance of being re-elected in 2023.
* Average rent of a SF 1BD, in $/ft2 in the year 2024, will be $6.00. [Halfway between $2 and $10].

#### D. The Subsidy

Once the market has been created, it is trivial[^1] to introduce a small **subsidy** -- money that is in the market but that does not own any shares. This could be as little as $5000 or $10000.

Then, profit seeking traders will buy whichever states they think are too cheap. Even if there is only **ever** one single trader, that trader can still make trades that will eventually win them the entire subsidy.

[^1]: For details on how the subsidy works, see my [Excel LMSR Guide](http://bitcoinhivemind.com/papers/LogMSR_Demo.xlsx).)

#### E. Why would these prices be accurate?

A better question is to ask: why would they ever be even the slightest bit *inaccurate*? If there is ever any inaccuracy --about the likelihood of the mayor's election, about the rent in 2024, or about the relationship between these-- then it implies that at least one of the four shares are underpriced. Someone can earn money (unilaterally), by buying this underpriced share.

So whenever there is an inaccuracy, then a profit-opportunity is freely presented to the entire world.

For example, (as I mentioned above) the instant in which this market is created, it will have prices of (25-25-25-25), and therefore be estimating a 2024 rent of $6. However, SF Rent is [currently](https://www.apartmentguide.com/blog/cities-with-most-expensive-apartments-per-square-foot/) $5.73, and 2% inflation per year for four years would put it at $6.20. Thus, one would be inclined to buy the two right-most shares (these are the "rent goes higher" shares), one of each at a total cost of $0.50 (ie, $0.25 + $0.25). Because if the future rent ends up being $6.20 or higher, then the value of those shares will be worth $0.525 (regardless of who wins the election). Thus, a return on investment of +5% for each dollar invested.

The larger the error corrected, the higher the return on investment. So the market is, in effect, continuously paying you to fix its errors.



#### F. How Long Will it take to see results?

The average 2024 rent, won't even be measurable until some time in 2025 (as the data needs time to be collected and published). While people can buy and sell at market prices at any time, the market cannot possibly "settle up" with everyone until after this date in 2025. That's a long time!

Does that mean that rents will continue to be arduously high, until 2025?

No.

If politicians believe that they will be evaluated on this metric, they will start to focus their energies on the metric immediately (just as today's politicians are always focusing their daily energy on winning the next election). In particular, if the current Mayor can start a multi-year project that reduces future rents in 2024, she will do so (as long as she can dismantle the project, if she loses the 2023 election, to prevent her rival from getting any credit for it).


#### G. What about manipulation?

Believe it or not, manipulation is really not possible in this scheme.

If the mayor purchases millions of dollars of lower-left shares, for example (so as to make it appear that by keeping the Mayor, rents will be low), then they may "buy" their way into re-election.

But the problem is that they are now holding millions of dollars worth of shares that will be worthless, if the *actual measured rents* end up being high (and not low). They have won the election, but have not yet escaped accountability. They merely traded accountability to the voter, for accountability to the rent-metric.

Meanwhile, all of her critics and skeptics (and, likely, shrewd political rivals) will be holding the opposite shares (which, as a direct result of the "manipulation", are much cheaper). So, if the mayor wishes to "buy" re-election, she may need to spend an unlimited amount of money to do so, and all of this money will go directly to her political rivals when she ultimately fails to deliver lower rents. To buy the election, she must be prepared to lose an unlimited amount of money.

It is not at all like the political scams of the past. Here, the mayor can only keep her money, by keeping her word.

#### H. Other Thoughts

In a city with more landlords than renters, the public may instead want *higher* rents, and elect whichever mayor drives rent *up*!

On utilitarian grounds, the scheme works pretty well -- there are more owners than renters, so the owners get what they want (and renters do not). It isn't as though the "bad guys" are exploiting "political organization" to win, instead they're winning fair-and-square by being a majority. Renters would have to flee to a nearby commuter town (where the majority of the electorate rents). When they're ready to buy, they should move back to the high-rent town.

Isn't this democracy just a tyranny of the majority?

The mayor might increase rents in "evil" ways, like restricting supply. Or she might do it in "good" ways, by making sure there are lots of great schools, parks, and jobs nearby.

As argued by Henry George long ago, the optimal tax is a [land value tax](https://en.wikipedia.org/wiki/Land_value_tax). The optimal metric for assessing a government, is changes in land-value. So taxes should be based on some (small) percentage of land value, and people should elect the government which improves land-value the most.

This small blog post, covers just one instance of a wider problem (that laypeople lack information on how their vote affects economic variables [such as rents]).

#### Conclusion

Was this post simple? Let me know.

---

### Footnotes

