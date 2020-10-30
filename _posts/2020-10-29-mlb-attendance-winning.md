---
layout: post
title: The Relation Between Home Game Attendance and Winning Percentage in MLB
date: 2020-10-29 18:50:22 -0300 
use-site-title: true
comments: true
archive: true
subscribe: true
image:
tags:
- MLB
- Attendance
- Winning percentage
- NFL
---

I came across a post on the *Data is Beautiful* <a href = "https://www.reddit.com/r/dataisbeautiful/" target = "_blank">subreddit</a> showing <a href = "https://www.reddit.com/r/dataisbeautiful/comments/ji2yzs/oc_updated_nfl_attendance_adjusted_for_stadium/" target = "_blank">NFL home game attendance</a> over the last 20 years and wondered how it has looked in Major League Baseball. So I grabbed team schedules and results, and playoff appearances and successes (i.e., winning league pennant, winning World Series) from <a href = "https://www.baseball-reference.com/" target = "_blank">Baseball-Reference.com</a>, tabulated MLB stadium capacities from their respective Wikipedia pages, and then put it all together to generate the graphic:

<center><a href = "/img/posts/20201029/fig1_allMLB_1999-2019.pdf" target = "_blank"><img src = "/img/posts/20201029/fig1_allMLB_1999-2019.svg" width="85%"></a></center>

<p style = "text-align: right; font-size: 45%; margin-right: 10%">(<em>click image to embiggen</em>)</p>

One thing that jumped out to me is the lack of consistently *filled* stadia in MLB, especially relative to the NFL. Only the Red Sox have consistently played in front of a filled (or very close to filled) stadium. The stadium capacities in the NFL tend to be higher than those in the MLB and yet many NFL teams fill their venues each week. Of course filling a stadium eight times is easier than filling a stadium 81 times, regardless of team quality. The New England Patriots can put 65,878 folks into <a href = "https://en.wikipedia.org/wiki/Gillette_Stadium" target = "_blank">Gillette Stadium</a> eight times a year, but an MLB team only needs to get 6,506 people through the gates every home game to match the overall attendance. Both the lowly Rays and Marlins, known for <a href = "https://www.cteeter.ca/blog/2019-11-26-attendance-baseball-florida-giancarlo-stanton-hr/" target = "_blank">lacking fans in the stands</a>, outdrew the Patriots in 2019. 

The second thing that can be gleaned from the figure above, although not easily, is the relationship between team performance and attendance. It is reasonable to expect that when a team is playing well more people will come to watch them play, and vice versa. However the strength of this relationship can vary. For example, the Tigers' and Royals' home attendance has been strongly related with winning:

<center><img src="/img/posts/20201029/fig2a_attend_by_winPCT_TigersRoyals.png" width="80%"></center>

While the Reds' and Athletics' attendance has not:

<center><img src="/img/posts/20201029/fig2b_attend_by_winPCT_RedsAthletics.png" width="80%"></center>

I am interested in seeing how these trends evolve over the next five to ten years. More and more we have seen a decoupling of team performance and revenue, as things like revenue-sharing, local and national television deals, and MLB Advanced Media provide teams with significant streams of money that make them less dependent on ticket sales.

***

A .csv file with the correlation coefficents between home attendance and winning percentage by team for the 1999 to 2019 seasons is <a href = "https://www.dropbox.com/s/zjx9m3c00bi76cy/team_attendance_by_winPCT_rvals.csv?dl=1" target = "_blank">here</a>.

The history of attendance and winning percentage for a single team (back as early as 1969) can also be interesting. For example, the <a href = "/img/posts/20201029/fig3a_RedSox.png" target = "_blank">Red Sox</a>, <a href = "/img/posts/20201029/fig3b_BlueJays.png" target = "_blank">Blue Jays</a>, <a href = "/img/posts/20201029/fig3c_Dodgers.png" target = "_blank">Dodgers</a>.