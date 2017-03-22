---
layout: post
title:  "Granular Data"
date:   2017-03-01 09:45:12 -0600
categories: jekyll update
---

Granular Data for SVS

Currently, STATS collects a lot of data that no other business collects. The way we currently collect the data is through our Ops department; specifically through part-time employees and reporters that are either "in-house" or "out of house".

In-house reporters are currently employees at STATS. They aren't necessarily in the Ops department, but many of them are. Out of house reporters may have worked at STATS previously, but it's not a requirement. The only requirement is that you get certified through a process that involves studying and testing. The amount of studying and testing depends on the sport you are attempting to get certified for.

The only reason the above information is important for collecting granular data is that there is a level of expertise required to be certified. We don't want to collect a bunch of data only to determine that it isn't useful at another time. A good example of that would be our STATS bunt attempts data. Currently we have a lot of common data collection on bunt attempts. Was there a bunt attempt, was it a fair/foul ball, was it a sacrifice bunt, etc. That's data that is collected by many sources. The way we could differentiate ourselves in the baseball metrics world would be to go back through all of the bunt attempts and add additional information to each event. Was it a drag bunt attempt? Was it a pull/push bunt attempt toward the right side. What is the "success rate" of each bunt attempt?

Once we get all the types of data that we want to collect, we would need to determine the most useful and practical way to store it. Whether it was in an Excel spreadsheet or straight to an empty database table, we could easily gather thousands of new data points. The best way to collect it is by using our in-house part-time employees in the Ops department. Here's the steps that we would need from developers to set up the Ops guys:

First, we would need a query that would give a list of the Player, date, and inning of all bunt attempts as far back as we would want to go. We should probably categorize it by team to make it easier to gather the data.

Second, we would need to put that list in a formatted table that would also have the different types of data that we want to collect as the headers of the columns.

After that, the Ops team could use SVS to review each bunt attempt and add the additional data points with a simple Y/N or 1/0. Once all of the data was collected, we would need to somehow hook it in to SVS for clients to easily read/check out.

3-15

I learned today that we incorporate more than just SQL to get our front-end results for bunts. But I learned what the different SQL rows, strings, and IDs are, so I can now query any range of games within Oracle to get all the events that we consider "all bunt attempts".  With that, I want to create a spreadsheet with all bunt attempts, date, player, etc. and see if I can definitively categorize them with more granular data such as drag, push, bunt for hit, etc. I think the best way to figure out what categories (extra info) data we can add to it would be to just dive in and see what I can discover through manually labeling them. If I can create a decent sales pitch out of that, I might be in good shape. My end goal here is to have a decent sales pitch to the Ops Managers, so we can start using our reporters to chart x-info bunt data.

The problems we run in to here is essentially the difference between qualitative and quantitative data. Qualitative data isn't considered 
