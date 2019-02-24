---
layout: page
title: Applications
subtitle: A collection of Shiny apps I have developed
use-site-title: true
show-avatar: true

---

<style type="text/css">
table {
	width: 100%;
}
tr, td {
	border-top: 1px solid #ddd !important;
	border-bottom: 1px solid #ddd;
	padding: 25px 13px 25px !important;
}

.imgshadow {
	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
	text-align: center;
	transition: all 0.3s ease-in-out;
}

.imgshadow::after {
	z-index: -1;
	opacity: 0;
	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
	text-align: center;
	transition: opacity 0.3s ease-in-out;
}

.imgshadow:hover {
	transform: scale(1.05, 1.05);
}

.imgshadow:hover::after {
	opacity: 1;
}

</style>

<br/>

<table>
    <colgroup>
       <col span="1" style="width: 35%;">
       <col span="1" style="width: 65%;">
    </colgroup>
    <!-- The Masters Row -->
        <tr>
            <td style="text-align:center" bgcolor="white"><div class="imgshadow"><a href = "https://cjteeter.shinyapps.io/MastersGolf/" target = "_blank"><img src="{{site.url}}/img/app3_mg.png" alt="Masters Golf"></a></div></td>
            <td bgcolor="white"><a href = "https://cjteeter.shinyapps.io/MastersGolf/" target = "_blank"><b>The Masters</b></a> offers users a tool to explore and visualize the history of <i>The Masters</i> golf tournament. Among other things, you can see whether scores have changed over time, play with aggregated historical leaderboards, and review players' scoring averages.</td>
        </tr>
    <!-- MLB Team Synchrony Row -->
        <tr>
            <td style="text-align:center" bgcolor="white"><div class="imgshadow"><a href = "https://cjteeter.shinyapps.io/MLBTeamSynchrony/" target = "_blank"><img src="{{site.url}}/img/app2_ts.png" alt="MLB Team Synchrony"></a></div></td>
            <td bgcolor="white"><a href = "https://cjteeter.shinyapps.io/MLBTeamSynchrony/" target = "_blank"><b>MLB Team Synchrony</b></a> uses major league baseball data from 1998-present to allow users to examine how run scoring and run prevention vary over the course of a season, and how these can be <i>in-sync</i>, leading to periods of consistent results (wins or losses), or <i>out-of-sync</i>, leading to a one-step-forward-one-step-back feeling.</td>
        </tr>
    <!-- Decision Maker Row -->
    	<tr>
    		<td style="text-align:center" bgcolor="white"><div class="imgshadow"><a href = "https://cjteeter.shinyapps.io/DecisionMaker/" target = "_blank"><img src="{{site.url}}/img/app1_dm.png" alt="Decision Maker"></a></div></td>
    		<td bgcolor="white"><a href = "https://cjteeter.shinyapps.io/DecisionMaker/" target = "_blank"><b>Decision Maker</b></a> takes input on options for a decision you are trying to make and returns a randomly selected choice. It is intended for people like me who perpetually overthink simple things.</td>
        </tr>
</table>

<br/>

Please [contact me]({{site.url}}/contact/) if an application is not working and/or you have suggestions for improvement.