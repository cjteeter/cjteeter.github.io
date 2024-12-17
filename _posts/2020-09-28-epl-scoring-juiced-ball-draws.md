---
layout: post
title: The Juiced Ball Comes to the EPL [Updated]
date: 2020-09-28 10:07:09 -0300 
use-site-title: true
comments: false
archive: true
subscribe: true
tags:
- English Premier League
- Tottenham
- Scoring
- Draw percentage
---

This year, more than ever before I have committed to watching and following the English Premier League (EPL). The EPL has always been relevant in my family but just hasn't ever been a focus for me. I would name "my team" if asked (Tottenham, Wolverhampton for a year or so before they were demoted) but it was an empty support. Now, perhaps COVID-19 related or Major League Baseball's ongoing effort to make me dislike their product, I am in. Just this past weekend I was swearing at my television because of a <a href = "https://en.wikipedia.org/wiki/Video_assistant_referee" target = "_blank">Video Assistant Referee</a> (VAR) call that stole a win from my (yes, _my_) Spurs. Expressing anger over VAR felt like a rite of passage.

Along for this newfound interest of mine is my brother. He is a huge soccer fan, a huge Arsenal fan, an excellent midfielder, and has been more than generous with his time in responding to all of the questions and comments I fire at him about the game, strategy, players, coaches, and rules. Learning from him has been great. Ideally it will inform my shit-talking about The Gunners on <a href = "https://www.premierleague.com/match/59003" target = "_blank">December 5</a>.

During one of our recent conversations he suggested that there had been a lot more scoring this year than was typical. Being that I am primarily a baseball fan, I made a joke about the EPL having introduced <a href = "https://www.cteeter.ca/blog/2019-11-29-home-run-surge-baseball-drag/" target = "_blank"> _juiced balls_</a>, but said I would look into scoring data to see if it was truly the case. <a href = "https://fbref.com/en/comps/9/Premier-League-Stats" target = "_blank">Football-Reference.com</a> has scores and fixtures for the EPL going back to 1992-1993. I grabbed everything since the 2007-2008 season and then compared the average goals per match across seasons (limited to the first three weeks, as we are only three weeks into the 2020-2021 season). Seems my brother was right:

<center><img src="/img/posts/20200928/fig1a_EPLscoring_first3.png" width="78%"></center>

Through the first three weeks of this season there has been an average of 3.68 goals per match, which is almost a full goal more than last season's average (2.73) through the same period, and easily more than a half-a-goal more than the next highest season (2018-2019: 2.97). Maybe the balls _are_ juiced.

My brother also felt that there were fewer draws than is typical. Again, he was on it. There have only been two draws through the first three weeks of the 2020-2021 season. Other than 2009-2010 in which there was only one draw in the first three weeks, this year has seen the lowest percentage of drawn matches:

<center><img src="/img/posts/20200928/fig2_EPLdraws_first3.png" width="78%"></center>

It could be that these two things are related. In an effort to shorten games and reduce the likelihood of 14+ inning games, Major League Baseball implemented a new extra innings format in which teams start each extra inning with a runner on second base. You might think that because each team gets the same benefit this would not change the outcomes. Both teams will easily score the free runner and things will remain tied. But the effect of the free runner is to increase the _variance_ in run scoring for the inning. Teams are now more likely to score multiple runs and it is less likely that both teams will score the same number inning-after-inning. Perhaps something similar is happening in the EPL this year. Scoring is considerably higher (and more variable) and this is limiting the number of draws. That sounds nice and to some extent lines up with what is going on in baseball's extra-innings, but there isn't much of a relation between average goals per match and percentage of draws (_r<sup>2</sup>_ = 0.09).

Maybe the delayed start to the season and/or the lack of fans in attendance has something to do with the differences in these measures this season. Or it is just a random blip. Regardless, I am probably going to be tracking things over the coming weeks. If they regress to typical levels we could be in for a spate of low-scoring draws, which sounds much less fun.

***

*__Update__* (October 20, 2020)

After five weeks the 2020 EPL season continues to be a scoring outlier:

<center><img src="/img/posts/20201020/fig1a_EPLscoring_first5.png" width="78%"></center>

After five weeks, we are seeing an average of 3.58 goals per match, which is down a bit from the mark at three weeks, but still well above previous years. This season is the only one (at least since 2007) to average more than three goals per match after five weeks.

Since 2017, <a href = "https://fbref.com/en/comps/9/Premier-League-Stats" target = "_blank">FootballReference.com</a> has published <a href = "https://fbref.com/en/expected-goals-model-explained/" target = "_blank">expected goals</a> (xG) for each team for each game (and over the season). The expected goal data come from <a href = "https://statsbomb.com/" target = "_blank">StatsBomb</a>. The basic concept of expected goals is that any shot a player takes has some likelihood of scoring given a set of characteristics (e.g., location, foot/head, defenders). A player in a crowd of defenders, shooting 21m from the goal? Not likely to find the back of the net. A player standing 1m from the goal without a defender within 2m? That is almost certainly going to be a goal. Sum all of these likelihoods over the course of a game and you get an expectation for how many goals a team _should have_ scored given their opportunities. Caution is required when looking at expected goals for any single game but when aggregated over many games (and many teams) it offers a useful indication of how teams _should be_ performing. Consistently getting high-likelihood-goal chances is a good sign for a team's future even if so far those good chances have not been converted into goals. And the opposite is also true. Teams may have been unusually fortunate in scoring on lower quality chances and could be in for a decline in scoring. 

In 2020, EPL teams are scoring well above expectation:

<center><img src="/img/posts/20201020/fig4a_EPLscoring_AvX_first5.png" width="78%"></center>

Typically teams don't deviate too much from their expected level of scoring. Not so in 2020. In 2020 teams are scoring 0.78 more goals per match than expected, which is more than double the difference observed last season (0.35). 0.78 goals might not sound like much, but it amounts to 37 *extra* goals over the 48 games.

It is important to note that the *quality* of chance (i.e., expected goals) has not varied much over these four seasons. It is just that for some reason -- juiced balls? -- in 2020 teams are getting more from their opportunities. 

This xG analysis is still only descriptive. Players are finding ways to get their shots, even lower-quality ones, past keepers. But why this is happening remains unclear. The xG model from StatsBomb has been fairly accurate. I know it looks like it has been getting worse season-over-season in the figure above, but when using <a href = "/img/posts/20201020/fig4b_EPLscoring_AvX.png" target = "_blank">full seasons</a> the error has actually been decreasing season-over-season. To me, unless there is some major scoring factor that has changed, this suggests we are in for a few weeks of low-scoring (and underperforming expectation) games.

--

At <a href = "https://fivethirtyeight.com/" target = "_blank">FiveThirtyEight</a>, Ryan O'Hanlon looked into the <a href = "https://fivethirtyeight.com/features/why-has-premier-league-scoring-skyrocketed/" target = "_blank">EPL scoring boom</a> (even making a juiced ball joke!) and came to a similar shoulder shrug in explanation. He beat me to getting this xG analysis out, but it is reassuring to be on a similar track.