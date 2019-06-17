---
layout: post
title: How Has the NBA's 3-Point Obsession Impacted the Region?
subtitle: The NBA is getting smaller, faster, and prioritizing shots from farther away. Can the same be said about the D2 east region?
bigimg: /img/KeenanIMG0191.jpg
image: /img/header.png
tags: [D2 East Hoops, Data Science, Python, Plotly]
comments: true
---

Over the last decade, the NBA has gone through a rather extreme makeover. Thanks to transcendent stars like Steph Curry and James Harden, coaches have begun to prioritize three point looks over paint touches. I couldn't help but wonder how, if at all, this new era of the professional game has impacted play at the D2 level.
<!-- more -->

First, I decided to plot each basic three point metric by season. The third metric represents 3-point field goal percentage, while the fourth is the percentage of all field goals taken from behind the arc. For example with a percentage of 50, the team has taken 50 3's for every 100 attempted field goals. This is stat will likely be similar to 3-point attempts, however it is helpful because it removes pace of play from consideration.

You can click the dropdown on the left to sort by conference, double click on a team on the right to isolate that specific team, or single click on a team to add/remove. Note that these visualizations were intended to be viewed on a larger screen ie a desktop or tablet, so they might be difficult to view and interact with on a mobile device.

<iframe src="https://plot.ly/~millere680/2.embed"
        height="1000" width="100%"
        scrolling="no" seamless="seamless"
        frameBorder="0">
</iframe>


A few interesting things of note:

**Coaching Philosophies**

In some instances, you can easily spot which seasons a new coach has been hired. David Duke (Adelphi), Patrick Beilein (Le Moyne), and Michael Harding (Assumption) led their respective teams to huge spikes in three point attempts during their first year campaigns in 2015-16. While David Duke continues to lead the three point revolution in the NE10, it will be interesting to see which direction rookie head coaches Nate Champion (Le Moyne) and Scott Faucher (Assumption) will take their programs into the 2019-20 season and beyond.

Another interesting case is Saint Rose, where in 2017, Mike Perno took over for Brian Beaury after 32 years with the Golden Knights. The jump in threes per game between Beaury's final season and Perno's rookie campaign (+6) isn't as staggering as the previously mentioned coaches. The interesting bit here however comes in 2014-15, where the Golden Knights experienced another spike in attempts. The reason? Perno's first real experience leading the team, where he served as an interim coach for the full length of the season.

Region mainstays Jay Lawson (Bentley), Keith Dickson (Saint Anselm), Stan Spirou (Southern NH, 2008-2018), Gerald Holmes (Bloomfield), Joe Clinton (Dominican), and Mike Ruane (Bridgeport) have largely been consistent on this front over the past decade. The latter mentioned Holmes, Clinton, and Ruane's squads have seen a bit of a jump in attempted 3's over the recent seasons, while Lawson, Dickson, and Spirou have been a bit ahead of their time in the NE10 with consistently high shot attempts since 2010.

**Record Highs and Lows**

When looking at the graphs, Adelphi and Holy Family's gaudy numbers really jumped out at me. These are the only two teams in the region who have average over 30 attempted threes per game in a single season, both having done so a combined six times. The results over these six seasons have been a bit of a mixed bag for both teams, combining for a 94-81 record (.537) with one NCAA tournament appearance.

Adelphi (2015-16): 11-18  
Adelphi (2017-18): 20-9  
Holy Family (2014-15): 22-8  
Holy Family (2015-16): 26-6 (NCAA #1 Seed)  
Holy Family (2016-17): 11-17  
Holy Family (2017-18): 4-23  

On the opposite end of the spectrum is USciences, who spent six consecutive seasons at the bottom of the CACC's list of threes attempted. Prior to the 2014-15 season, seven teams posted seasons with less than 12.5 threes per game. Beyond 2014-15, the 12.5 mark has only been missed four times, three of which came from USciences. Surprisingly though, these four seasons saw a combined record of 66-49, one tournament berth, and a win percentage four points higher than the previously mentioned 30+ 3PA/G teams.

Assumption (2014-15): 8-18  
USciences (2014-15): 25-6 (NCAA #6 Seed)  
USciences (2015-16): 17-12  
USciences (2017-18): 16-13  

Next up, a look at the league wide trends for all three conferences in the region. I added statistics from the NBA to better understand how the regional trends match up with the professional game, and adjusted them to be on a per 40 minute basis instead of 48 for a better comparison to the NCAA.

<iframe src="https://plot.ly/~millere680/4/"
        height="600" width="100%"
        scrolling="no" seamless="seamless"
        frameBorder="0">
</iframe>

Each metric, with the exception of 3-point field goal percentage, seems to be following a consistently positive trend for each conference. If you look back at NBA data before the 2008-09 season, 3-point attempts per year were on the rise by around 1-2 shots per game every couple of seasons, but nothing close to the rates seen today. I was expecting the region to be lagging a couple of years behind the NBA, but 3-point attempts in the D2 game seem to begin picking up steam around the same time as the NBA during the 2012-13 season.

Overall, these numbers are largely consistent with what you'd probably expect if you've been keeping track of the sport for the last handful of years. There are still however a few interesting observations, starting with the NE10's collective 3-point percentage. you'd probably assume that a large increase in shot attempts would lower field goal percentage, but the NE10 actually got better from behind the arc over the last decade. Perhaps this can be attributed to coaches placing a higher emphasis on recruiting 3-point shooters, and/or players focusing on adding the shot to their game as they try to make it to the college level.

When looking at percentage of 3-point field goals taken, the NBA is finally beginning to close the gap on it's college counterparts. As mentioned previously, this stat removes pace of play from consideration. The professional game, much quicker due in large part to a 24 second shot clock, has largely trailed the region for the past 11 seasons. While rates across the region have only shown moderate growth in the last 4-5 seasons, the NBA continues to take a higher percentage of their field goals behind the arc as the years go on. 

Moving along from the year to year trends, my next question was simple - how have these trends impacted the win column?

<iframe src="https://plot.ly/~millere680/6/"
        height="600" width="100%"
        scrolling="no" seamless="seamless"
        frameBorder="0">
</iframe>

While there does seem to be a positive correlation between 3-point attempts and win percentage, it isn't much. Essentially, for an average team, every five additional 3's attempted per game has been worth an additional win over the last 11 seasons. An interesting observation, but hardly compelling enough to convince coaches to start launching 50 3's per game. I decided plot NCAA tournament qualifying teams separately, as seen in red. The average 3-point attempts taken for these teams was just slightly under 21 per game, incredibly close to the region wide average of 20.

I wanted to take a closer look at these trends between teams that did and didn't qualify for the NCAA tournament each year, which resulted in the following graph.

<iframe src="https://plot.ly/~millere680/8/"
        height="600" width="100%"
        scrolling="no" seamless="seamless"
        frameBorder="0">
</iframe>

This shows that, while qualifying and non-qualifying teams have been following similar trends over the past decade, teams missing out on the tournament have recently closed the gap in 3-point attempts on their region leading counterparts. 3-point makes and percentage metrics have favored tournament qualifying teams in each of the last 11 seasons, but mostly by a small margin.

Finally, a look at how these stats have impacted wins on a single game basis. I took a look at 4,500 games across the region since 2008, which team led the game in each metric, and the outcome for the leading team.

<iframe src="https://plot.ly/~millere680/10/"
        height="600" width="100%"
        scrolling="no" seamless="seamless"
        frameBorder="0">
</iframe>

Over this time frame, teams have been hovering right around .500 when leading the game in 3-point attempts. Of course the 3-point attempts stat says nothing about the quality of shots taken in each game. You might assume that a team taking 11+ additional 3's would give teams more opportunities to put points on the board,  but it has actually caused them to perform a bit worse overall. This isn't completely surprising, as there were probably a lot of cases where a team started throwing up 3's to make up for a large early deficit.

Not as surprisingly, made threes and high shot percentages have clearly been important to a successful outcome. Teams making 3+ additional 3's have won 67.8% of their games, while teams shooting at least 10% better than their opponents from behind the arc have posted a 77.6% win percentage. 

In instances where one team led the game in three point makes and the other shot a better percentage from long range, over the course of 1,021 games, the teams shooting a higher percentage have won 64.2% of the time. One great example of this came when Holy Family and USciences, two teams previously noted for their wildly contrasting styles, squared off in 2017. Despite an incredible barrage of 3's, Sciences edged out a victory on the road with consistent, higher percentage shooting.

| Team         | 3PM     | 3PA  | 3P% | Score |
|:------------:|:-------:|:----:|:---:|:-----:|
| Holy Family  | 6       | 9    | 67% | 85    |
| USciences    | 14      | 40   | 35% | 81    |

Overall, the data largely seems to be in line with conventional thinking about the modern game. 3-point statistics have been consistently on the rise for much of the last decade, and more made shots and efficient shots lead to more wins. I wanted to learn more about the impact of attempted 3's, as that's one of the few things within the control of a coach, but whether or not a team is better after taking more shots still remains to be seen. 

For future consideration, I'd like to take a deeper look at 3-point attempts and provide more context to some of the above graphs. As mentioned earlier, it's possible that teams often take more 3's when trailing, causing them to take shots that are forced and inefficient.

All data and code used in creating this article can be found on my Github account [here](https://github.com/emiller518/emiller518.github.io/tree/master/code/Region3PointAttempts).

