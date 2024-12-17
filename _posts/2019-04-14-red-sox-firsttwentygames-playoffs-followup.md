---
layout: post
title: The Probable (Hopeful!) End of a Red Sox Fun Fact
date: 2019-04-14 05:10:29 -0300
use-site-title: true
comments: false
tags:
- Playoffs
- Red Sox
- Early season panic
---

The Red Sox have started the season poorly. Their sloppy, pressing play has resulted in a 5-10 record (-29 run differential). It is only 15 games, but that record is ominous. No Red Sox team has ever made the playoffs after posting a sub-.500 record in their first 20 games. This silly bit of trivia is something <a href = "https://christopherteeter.wordpress.com/2014/05/13/playoff-chances-after20/" target = "_blank"> I have tracked</a> over the <a href = "http://boston.locals.baseballprospectus.com/2015/04/27/crossing-the-first-hurdle-playoff-chances-after-20-games/" target = "_blank">last few years</a>.

For whatever reason (likely the randomness inherent to baseball), getting a 10th win in the first 20 games of the season has been an important benchmark for this franchise. Since 1903, Red Sox teams have made the playoffs 25 times in their 116-year history -- 21.55% of their seasons, which is seventh best among all franchises since 1903 -- but none of those playoff seasons came after a 9-11 (or worse) start. And it is not for lack of 9-11 (or worse) seasons. The Red Sox have posted 46 such starts.

Here is the distribution of win totals in the first 20 games for all franchises (since 1903; all data from <a href = "https://www.baseball-reference.com/" target = "_blank">Baseball-Reference</a>):

![Fig1_WinsHistogram](/img/posts/20190414/fig1_winsHist.png)

It is also important to note that the Red Sox franchise is not alone in, or even the worst example of, this ignominy:

<table style="width:80%" align="center">
<tr> <th style="text-align:left" bgcolor="gainsboro"> Franchise </th> <th style="text-align:center" bgcolor="gainsboro"> Seasons with a sub-.500 Start (in First 20 Games) and No Playoffs </th></tr>
  <tr> <td style="text-align:left" bgcolor="white"> Baltimore </td> <td style="text-align:center" bgcolor="white"> 63 </td> </tr> 
  <tr> <td style="text-align:left" bgcolor="white"> Boston </td> <td style="text-align:center" bgcolor="white"> 46 </td> </tr> 
  <tr> <td style="text-align:left" bgcolor="white"> Seattle </td> <td style="text-align:center" bgcolor="white"> 22 </td> </tr> 
  <tr> <td style="text-align:left" bgcolor="white"> Milwaukee </td> <td style="text-align:center" bgcolor="white"> 19 </td> </tr> 
  <tr> <td style="text-align:left" bgcolor="white"> Washington </td> <td style="text-align:center" bgcolor="white"> 19 </td> </tr> 
</table>

Other franchises have had plenty of sub-.500 starts in their first 20 games, but have made the playoffs in at least one of those years. The five franchises above are the only ones who have never made the playoffs in a season that started 9-11 or worse. Baltimore will likely add another notch to this table this year, Seattle and Milwaukee already have 13 and 9 wins, respectively, so their counts won’t increase, and then there is Boston and Washington. Both have struggled out of the gate this year, but both are considered strong playoff contenders, so maybe this is the year they remove themselves.

Here is the full picture of this trend between making the playoffs and early season record:

![Fig2_PostSeasonPlot](/img/posts/20190414/fig2_pstPLOT.png)

Each point represents a franchise, with the size of the point scaled to the number of seasons the franchise has posted with the given win total in the first 20 games (bigger points = more seasons of that win total). The line is a <a href = "https://en.wikipedia.org/wiki/Local_regression" target = "_blank">Loess regression</a>. The <a href = "https://www.baseball-reference.com/teams/BAL/1988.shtml" target = "_blank">1988 Baltimore Orioles</a>, who went 0-20 to start the year are not included. Unsurprisingly, more wins in the early going is related with a higher proportion of playoff appearances. You can also see the stark jump for the Red Sox from 9 to 10 wins that I have been discussing.

Since 1903, 10.9% of the 348 nine-win (in first 20 games) non-Boston Red Sox teams have gone on to make the playoffs. At 10 wins it is 13.8% (of 363 teams). Red Sox teams are 0% and 33.3%, respectively. You can see what I mean about the importance of the Red Sox getting that 10th win before their games played total flips to 21; something they are unlikely to do this year.

Making the playoffs is a somewhat arbitrary (and strict) measure of success. It depends on the performance of other teams, and even the rules of the league (e.g., there were no Wild Cards before 1994). So rather than restricting this analysis to playoff appearances, I could have used a team's win percentage after the first 20 games as the measure of success. Does a team’s winning percentage in their first 20 games predict their winning percentage over the rest of their games? A little bit:

![Fig3_WinPctPlot](/img/posts/20190414/fig3_winPCT.png)

Each point is a team’s season (n = 2,464). As you can see, good teams tend to play well and bad teams tend to play poorly. However, sometimes teams start poorly but then play well over the rest of the season (top-left quadrant); including some of those non-playoff Red Sox teams on whom I have been focusing, which highlights how limiting things to playoffs appearances gets us a fun fact but doesn't accurately describe how the team's season played out after Game 20.

All in all, this is a bit of early season fun that I have been over-analyzing since I heard it mentioned on a radio broadcast a few years ago. I don’t think there is really anything all that special about the first 20 games of a season. We should avoid overreacting to a team’s performance in the early going; let the season breathe. With this preached, why am I following up on this early-season panic again? Because the 2019 Red Sox are, on paper, pretty clearly one of the five (maybe three) best teams in the American League. So it is likely that they will make the playoffs this year, despite the ugly start. If they do, and obviously I really hope they do, it will mean the end of this fun fact, so I wanted to take one last look. 

Hopefully the 2019 Red Sox end up in the top-left quadrant of that third figure and end the franchise's <em>seasons with a sub-.500 start (in their first 20 games) and no playoffs</em> streak at 46.

***

*__Update__* (September 24, 2019)

They ended up going 7-13 over the first 20 games of the season and continued to play inconsistently the rest of the way. They will not make the playoffs in 2019, having officially been eliminated last Friday. So this silly fun-fact remains alive; the streak is now at 47. 