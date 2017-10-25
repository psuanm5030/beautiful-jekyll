---
layout: post
title: How did I spend my time in 2016? A RescueTime Data Analysis
tags: [rescuetime, efficiency, tableau]
image: /psuanm5030.github.io/img/rescuetime_01.png
---

In 2016, I had a lot going on, from taking on new responsibilities at work to trying to meet my continuous learning objectives (bettering myself with tools like python, R, and understanding other disciplines of data – e.g., databases, APIs, visualization).  This translated into spending a lot of time on my computer.  So, as we transition into this new year, I wanted to take a closer look at the data that was collecting through [RescueTime](https://www.rescuetime.com/).  If you aren’t familiar, it’s pretty simple.  RescueTime installs a lightweight application on your computer (in my case, both my work computer and my MacBook), then basically reads the “title bar” of the application you are working with, reporting this information back to my account, where it’s supplemented with metadata – such as category type (e.g., think “shopping” or “business communications”) and productivity classification (from very distracting to very productive).  This metadata is of course customizable (some people may think that email is “very productive” (not me – I think it’s distracting).  

Now RescueTime has some basic ways to “slice-and-dice” your data, with the abilities to change the time period or categories , as well as to view your productivity.  This was nice for a day-to-day baseline, but I wanted to dig deeper.  In order to do that I needed to:  

1. Acquire the data easily (and in a manner that didn’t take a large effort each time I wanted to update my visuals)
2. Understand and cleanse my data (sometimes time spent in Microsoft OneNote is logged as “ONENOTE” while other times it is “MS OneNote”).
3. Visually interpret my data (using my favorite tool – Tableau!)  
If you are only interested in seeing my visual analysis – scroll to the bottom!  

## Acquire the Data  

I started learning how to code with Python back in 2014 and love it.  It allows me to exercise my need to complicate things (note – I could have just downloaded a data file from RescueTime), while also allowing me to setup automation, customize everything, and munge (clean) my data.  

Therefore, I signed up for the API (once you’re a signed up – navigate [here](https://www.rescuetime.com/login?return_to=%2Fanapi%2Fmanage)) and wrote a lightweight python script to request certain data from RescueTime’s API and push it to a CSV file to later be consumed into Tableau.  It simply makes a request of the API, which returns a JSON object, which I parse (do some limited cleansing and organizing), and send to a CSV file.  

You can head on over to [my GitHub page](https://github.com/psuanm5030/Blog/tree/master/RescueTime) if you want to clone the repository and try it for yourself (you’ll need python – those steps are out of the scope of this blog post).  If you have no idea what I am talking about – check [this out](https://www.quora.com/What-does-it-mean-to-clone-on-github).

## Understand and Cleanse

Now that I have my data in a neatly organized table, I needed to understand and further cleanse it.  This is often one of the most time consuming steps in creating visual analytics, because **efficiently** visualizing the data requires that you understand what you are working with – meaning you should understand each and every dimension / measure, as well as how they interact together.

In my case, there was a specific hierarchy which was important: categories (e.g., “Data Visualization and Analytics”, “Email”, etc.) contained various activities (e.g., “Tableau”, “Outlook”, “Skype”), which also contained document level detail (e.g., the name of the “Tableau” file that was worked on or the subject line of the email written).  Other fields of importance where the date & time field (down to the 5 minute interval), productivity classification, and time logged (in seconds).

While this data was in a relatively simple structure, I took some time to ask questions of my data to see if it was what I expected – “Are all tableau activities linked to the right category?”, “What were my top activities?”, and “Does productivity make sense compared with what is reported in RescueTime?”.  After interrogating my data for some time, I realized that I had “Tableau” (my largest single activity) classified into two different categories (there were many other items like this).  I also needed to adjust for case with activities because Tableau is case-sensitive.  Finally, I needed to convert seconds into hours, because I was constantly recalculating in my head!  In the end, I ended up making changes to my category settings in RescueTime (and re-running my script) and created new fields in Tableau to cleanse, group and recalculate certain fields.  I could have done this in python, but it was far easier to do in Tableau.

## Visualize

Before I started actually building charts, I made a listing of key areas to investigate:  

* Understanding the undulations in logging over the year
* What did my “productivity” look like?
* What themes can be gleaned from categories?
* Looking at my year by activity – when and what did I get “focused on”?
* Are there important activities that I may not spent a lot of time in, but that are used frequently?
* Are there certain times or days with better utilization (or periods of time that )
* Doing this upfront, but after investigating my data, made my design process much more efficient and effective.  I was able to isolate the themes, then think about the metrics and charts that would speak to those.  Finally, I spent some time iterating on the actual charts and design, including significant time on layout, titles, and tooltips.  

Check out the finished product below, complete with my analysis and conclusions embedded within! (best viewed [here](https://public.tableau.com/profile/andy.miller#!/vizhome/RescueTimeAnalysis_0/TheMission))  

<iframe src="https://public.tableau.com/views/RescueTimeAnalysis_0/TheMission?:embed=y&:loadOrderID=0&:display_count=yes" height="1050" width="1000"></iframe>
