---
layout: post
title: "Time Series"
excerpt: "See all 4 dimensions (time) in Tableau visualizations"
tags: [apple, mac, setup]
shorturl: "https://goo.gl/8mGgPF"
image:
  feature: https://cloud.githubusercontent.com/assets/300046/14583248/4b20c578-03d9-11e6-8f7a-c860b666bc73.jpg
  credit: Wall Street Journal
  creditlink: http://graphics.wsj.com/job-market-tracker/
comments: true
---
<i>{{ page.excerpt }}</i>
<hr />

{% include _toc.html %}

Understanding metrics over time is a fundamental skill.

> "Those who don't know history are doomed to repeat it." -- Edmund Burke

## Excellence defined

Below are charts that posess traits of excellent visualizations:

 * Dynamic data - update visualizations (in "live mode") as data changes in sources such as databases. 
 
 * Visual querying -  change the query by selecting or clicking on a portion of the graph or chart (to drill down, for example). 
 
 * Linked multi-dimensional visualization - selections made in one chart are reflected as you navigate into other charts.
 
 * Animation -   

 PROTIP: Dynamic (movie mode) is available only within the Tableau Public client,
 not when viewed on websites (as of 2016-01-05).
 
 * Personalization - give power users an in-depth view and newbies a simpler view, and also control access to data based on user- and role-based access privileges.
  
 * Actionable alerts  -  thresholds and parameters that trigger messages whether you're interacting with reports or not. 


## Fortune 500 in the US

The higher each line is in their graph, the higher the company is on Fortune magazine's 500 largest public companies. 20 years of rankings are shown.

<a target="_blank" href="http://beta.fortune.com/fortune500/visualizations/">
http://beta.fortune.com/fortune500/visualizations<br />
<img width="1015" alt="dataviz time-series 2030x984" src="https://cloud.githubusercontent.com/assets/300046/24097787/cdd3b2f0-0d3d-11e7-889e-a99b161e1f55.png"></a>

Companies that have a rising trajectory include:

   * Whole Foods Market
   * Amazon
   * Alphabet (Google)
   * Apple
   * CVS Health
   * Comcast
   * Dollar General
   * Gilead Sciences
   * Qualcomm
   * Facebook
   * Visa
   * Master Card
   * Cognizant
   * Oracle

Select an industry and mouse over a line to see each company's Fortune 500 ranking change over the years.

<a target="_blank" href="http://nicolasrapp.com/">
Nicolas Rapp</a> also created for Fortune 500 this graphic:

<a target="_blank" href="http://nicolasrapp.com/portfolio/fortune-500-profits-run-gas/">
<img alt="dataviz-fortune500-oil-1120x772" src="https://cloud.githubusercontent.com/assets/300046/24098047/04c3dc1c-0d3f-11e7-9ec7-bc6d18022e8e.png"></a>


## Fortune Global 500

http://beta.fortune.com/global500/visualizations/?iid=recirc_g500landing-zone1

Illustrates the fast growth across industries in China.

Plus:

   * Softbank



## Hans Roling

  Since 2007 at
  http://www.gapminder.org/videos/
  Hans Roling, a professor of health statistics in Sweden, is
  an internet legend for his
  <a target="_blank" href="https://vimeo.com/18477762">
  "Joy of Stats" video</a> shown on BBC Nov 10, 2010 and Ted Talks.
  In them he shows his 
  <a target="_blank" href="http://www.gapminder.org/world-offline/">
  Gapminder web app</a> which
  presents multiple dimensions dynamically over time (nearly 300).

<a target="_blank" href="https://public.tableau.com/profile/jeffs8297#!/">Jeffrey Shaffer</a> 
(<a target="_blank" href="https://twitter.com/HighVizAbility">@HighVizAbility</a>, co-author of <a target="_blank" href="http://www.bigbookofdashboards.com/">bigbookofdashboards.com</a>) 
created <a target="_blank" href="https://www.youtube.com/watch?v=KdoBuNNvVec">
a time lapse video</a> of <a target="_blank" href="
https://public.tableau.com/s/profile/jeffs8297#!/vizhome/RoslinginTableau/RoslingGapminder">
his viz</a> showing a trail of dots which grow in size and get darker over time (as the legend notes):

<img width="599" height="379" alt="tableau time lapse gapminder" src="https://cloud.githubusercontent.com/assets/300046/12170866/a288bce6-b4f9-11e5-892b-d69d8cc35010.png"><!-- 1590x1006 -->

Here, different colors represent different countries, with the United States in red. Most other countries saw a decrease in fertility rate over time while life expectantcy increased.

Within the <a target="_blank" href="http://public.tableau.com/profile/andy.cotgreave#!/"> 
wonderful Tableau gallery</a>
Andy Cotgreave (<a target="_blank" href="https://twitter.com/acotgreave">@acotgreave</a>, now <a target="_blank" href="https://www.linkedin.com/in/acotgreave">Technical Evangelist at Tableau</a>)
built over the years is
<a target="_blank" href="http://gravyanecdote.com/andy-cotgreave/joy-of-six-gapminder/">
this re-creation of Gapminder</a>:

<img alt="tableau gapminder" src="https://cloud.githubusercontent.com/assets/300046/12102988/ba022edc-b2f3-11e5-8c2a-05c980223e21.png">

Andy
<a target="_blank" href="http://interworks.co.uk/blog/joy-of-six-gapminder/">
explained in 2010 how</a> he created the above using Tableau Trendalyzer v6.
<a target="_blank" href="http://public.tableau.com/profile/andy.cotgreave#!/vizhome/GapminderFullScreen/Gapminder">
Download his viz from the Tableau Public website</a> 
to manipulate using Tableau Public client installed on your laptop.

The trails is a recreation of 
(<a target="_blank" href="https://twitter.com/moritz_stefaner">@moritz_stefaner</a>)
"Remixing Rosling" in @tableau.


<a name="CycleTime"></a>

## Cycle Time  

<a target="_blank" html="https://cloud.githubusercontent.com/assets/300046/24077227/fc53a15c-0c1c-11e7-9782-9514f69c6a70.png">
<img width="978" alt="tableau interactive wait times 1956x1372" src="https://cloud.githubusercontent.com/assets/300046/24077227/fc53a15c-0c1c-11e7-9782-9514f69c6a70.png"><br />Click for full pop-up</a>

Metrics include:

* Percent of value-add time vs. total time.
   For example: In the case of physician visits, time interacting with physician vs. waiting and other activities.
   



## More on front-end styling #

This is one of several topics:

{% include front-end_links.html %}