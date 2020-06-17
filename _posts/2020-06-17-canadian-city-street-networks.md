---
layout: post
title: Comparing Canadian City Street Orientations
date: 2020-06-17 04:49:49 -0300 
use-site-title: true
comments: true
archive: true
subscribe: true
image: /img/posts/20200617/figx3_Halifax_ordinal.png
tags:
- R
- Maps
- Canada
- OpenStreetMaps
---

When I stumbled across Geoff Boeing's street network orientation visualizations for 25 major cities in the <a href = "https://geoffboeing.com/2018/07/comparing-city-street-orientations/" target = "_blank">United States</a> and 100 cities <a href = "https://geoffboeing.com/2019/09/urban-street-network-orientation/" target = "_blank">around the World</a> I made a note for myself to figure out how to (1) create something similar in R, and (2) do it for Canadian cities. Using polar histograms to demonstrate how a city's streets are oriented (in terms of compass bearings) is an interesting way to visualize the general pattern/structure of a city.

Boeing's posts and his article published in *Applied Network Science* (<a href = "https://appliednetsci.springeropen.com/articles/10.1007/s41109-019-0189-1" target = "_blank">PDF</a>) were really helpful for working out how to analyze and plot the street-level data. And <a href = "https://ggplot2tutor.com/streetmaps/streetmaps/" target = "_blank">this post</a> demonstrating how to use <a href = "https://www.openstreetmap.org/" target = "_blank">*OpenStreetMap*</a> data via the ```osmdata``` <a href = "https://docs.ropensci.org/osmdata/" target = "_blank">package</a>, was essential for getting everything coded in R.

I combined the concepts/instructions from those articles and was able to create a set of polar histograms for selected major Canadian cities. I chose 16 cities: the <a href = "https://en.wikipedia.org/wiki/Provinces_and_territories_of_Canada#Provinces" target = "_blank">ten provincial capitals</a>, the non-capital largest city (for the provinces in which the largest city is *not* the capital), and then Ottawa, Canada's capital. 

For each city I pulled the OpenStreetMap data (using default bounding box parameters) and used it to analyze the streets' bearings as Boeing described in his published article. Unlike the OSMnx software he used, the bearings of the streets are not given by osmdata. So to determine each street's bearing I relied on the ```geosphere``` <a href = "https://www.rdocumentation.org/packages/geosphere/versions/1.5-10" target = "_blank">package</a>, specifically submitting the start point and end point of the street (as defined in the set of nodes given in the OpenStreetMap data) to the <a href = "https://www.rdocumentation.org/packages/geosphere/versions/1.5-10/topics/bearing" target = "_blank">*bearing* function</a>. Doing it this way ignores the subtleties of mid-street curves or turns, but captures the overall bearing one would have to take to get from one end of the street to the other "as the crow flies". I then added the reciprocal of each street's bearing to account for the fact that streets point in both directions. For instance, if a street has a bearing of 45° then I add a bearing of 225°. In the analysis, each street is weighted by its length (<a href = "https://www.rdocumentation.org/packages/geosphere/versions/1.5-10/topics/distHaversine" target = "_blank">Haversine distance</a> from the start point to end point). This provides a cleaner representation of the city's *overall* orientation. Essentially, I didn't want Toronto's Yonge St. and Mill St. to hold equal sway on the overall representation of the city. All the bearings (and reciprocals) for all the streets in a city are then plotted as a polar histogram with 10° bins (centered on the 10s: 0, 10, 20, ..., 90, 180, 270).

So how well do these major Canadian cities follow the cardinal north-south-east-west orientation? Some more than others:

<center><a href = "/img/posts/20200617/fig1_allOrdinals_alpha.pdf" target = "_blank"><img src = "/img/posts/20200617/fig1_allOrdinals_alpha.svg" width="75%"></a></center>

<p style = "text-align: right; font-size: 45%; margin-right: 10%">(<em>click image to embiggen</em>)</p>

The direction of the bars in the polar histograms shown above represent the bearings of the streets and the length (height) of the bar represents the proportion of streets with those bearings. The concentric circles within each plot are in increments of 2%. So if a bar reaches up to the second circle it means that 4% of the streets in the city are oriented at that bearing. You can see that in, for example, Edmonton the streets are primarily oriented along the orthogonal N-S-E-W layout, whereas in somewhere like Fredericton, where I currently live, things are angled from that layout:

<center><a href = "/img/posts/20200617/fig2_Fredericton_combined.pdf" target = "_blank"><img src = "/img/posts/20200617/fig2_Fredericton_combined.svg" width="65%"></a></center>

<p style = "text-align: right; font-size: 45%; margin-right: 10%">(<em>click image to embiggen</em>)</p>

Most cities have a pretty strong orthogonal layout, even if it deviates from the cardinal directions, but places like St. John's and Halifax are exceptions. The streets in those cities are much more evenly distributed around the compass. Here's Halifax:

<center><a href = "/img/posts/20200617/fig3_Halifax_combined.pdf" target = "_blank"><img src = "/img/posts/20200617/fig3_Halifax_combined.svg" width="65%"></a></center>

<p style = "text-align: right; font-size: 45%; margin-right: 10%">(<em>click image to embiggen</em>)</p>

You can see that Halifax has areas that follow an orthogonal grid, but these grids are not aligned with each other, which explains the wider distribution of street orientations in the city. Other than St. John's, Halifax is the city that is least organized along one primary orthogonal grid. Here are all the city-histograms again, but rather than being ordered alphabetically they are ordered by the extent of their gridness, as determined by longest bar (from Vancouver to St. John's):

<center><a href = "/img/posts/20200617/fig4_allOrdinals_grid.pdf" target = "_blank"><img src = "/img/posts/20200617/fig4_allOrdinals_grid.svg" width="75%"></a></center>

<p style = "text-align: right; font-size: 45%; margin-right: 10%">(<em>click image to embiggen</em>)</p>

It is worth noting that my use of default bounding boxes for the cities affects things. This means that the comparisons are not *necessarily* apples-to-apples. In some cases wider areas are included and so the volume of streets can impact the proportions in the histograms. For example, Montreal is much less ordered than I expected it to be, but I suspect that is because a rather <a href = "https://www.openstreetmap.org/relation/1634158" target = "_blank">large area of streets is included</a>.  

Regardless of the imperfect comparisons of street networks, this was a fun way to explore some Canadian cities and develop tools for analyzing some new (to me) data in R. I also took time to look at the characteristics of cities not included in the figures above (e.g., <a href = "/img/posts/20200617/figx1_ThunderBay_combined.pdf" target = "_blank">Thunder Bay</a>) and also developed code to turn the map-with-histogram images into decent looking <a href = "/img/posts/20200617/figx2_Hamilton_Ontario_poster.pdf" target = "_blank">posters</a>. You can find the code for doing so <a href = "https://github.com/cjteeter/Rcode/blob/master/cityorientation_poster.R" target = "_blank">here</a>.