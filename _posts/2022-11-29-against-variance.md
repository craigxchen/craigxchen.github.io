---
layout: post
title: against variance
---

I'm worried that a message people may take away from this blog is just to maximize EV and eat all the variance they can. I like variance because higher risk often demands compensation in the form of higher expected return, but variance isn't always a good thing! The easiest example comes from, obviously, finance: variance drain. 

For starters, if you have two assets A and B where $$\mathbb{E}[A] = \mathbb{E}[B]$$ but $$\rm{Var}(A) > \rm{Var}(B)$$, then over time, asset A will generate *lower* returns than asset B. Of course in investing this is partly why we're interested in not just the return but the risk-adjusted return. To make this point excruciatingly clear, notice that if a stock starts out at $100, goes up 10% and then down 10%, the stock is actually now only $99. But the arithmetic average of the returns is 10% + (-10%) = 0%! In this case, the geometric average $$\sqrt(1.1 * 0.9) \approx 0.995$$ is a better approximation of the return. People who did competition math may recall the AM-GM inequality which states that the arithmetic mean (AM) is always greater than or equal to the geometric mean (GM) -- equality holds when all of the numbers in the average are the same. The point is, when we look at the cumulative return over many years, we see that we end up getting a return closer to the geometric mean rather than the arithmetic mean and this difference is what we call variance drain (aka volatility drag). 

If you want to estimate this quantity yourself, a common approximation is AM - 1/2 Variance = GM. This approximation is not the greatest but it's better than no estimate at all; to derive it, just expand the formula for the geometric mean to the second order in the returns and toss the rest. For more on this you can check out this [blog](https://breakingthemarket.com/the-most-misunderstood-force-in-the-universe/).

One last thing to note is that this effect comes from compounding. In many games, we're not necessarily betting the entire bankroll on every bet, so we actually do realize closer to the arithmetic average if we play many times. 

### ok, that's finance, why do I care?

It would be great to have an infinite bankroll, but no one does. In trading you quickly learn that hedging is bad, but then why do people still do it? 

Everyone has a risk tolerance, even clowns like SBF. At some point the variance is just too much to bear; if the variance makes you unhappy, then it's actually not +EV. I believe I've written it before, but it's so so important that you are calculating life/happiness EV when making decisions and not dollar EV. 

I personally find some stability in my life incredibly rewarding. While I was in college, there was a cafe I would go to every. single. friday. I went to the cafe each week around 11-12, ordered brunch and coffee while chatting with the baristas, asking about their days and what new coffees they were getting, and then read a book or worked on research, gazing outside, zoning out. Since I've moved to new york I've yet to find something similar. Sure, Fridays aren't possible anymore because I have a job, but each weekend I find myself grasping for something to repeat. I still go swimming most Sunday mornings, but that feels more like exertion than recollection of the self.

Especially in a city like New York, there's a lot of expectancy to trying new things since there is simply so much to try. However, it may turn out that compounded over many years, finding your home away from home may yield better returns.
