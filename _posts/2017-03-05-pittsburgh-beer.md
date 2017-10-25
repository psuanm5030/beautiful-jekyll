---
layout: post
title: Pittsburgh Craft Breweries
tags: [beer, untappd, tableau]
image: /psuanm5030.github.io/img/pgh_beer_01.png
---

I am not a crazy beer buff, but I think the scene in Pittsburgh is really interesting and unique. Currently, there are over 35 independent breweries in Pittsburgh! These aren’t just breweries, but these are venues, most of them including some form of outdoor element and food. It’s awesome. It makes Saturdays and Sundays so much more fun, as there is somewhere to go hangout and drink a good beer with friends and family – despite winter weather.  

One of the coolest websites out there is [Untapped](https://untappd.com/), which is a website focused on beer, breweries and venues that can be shared with friends. It includes elements of rating, checking into and generally sharing information about beer. Its amazing how people love to share their experiences, and when it comes to beer / breweries – this is great – because we all know that finding that right beer can sometimes be a guess-and-check affair. Personally, I follow my friend Alex, as he has a great affinity for beer and we tend to like the same types (sours!).  

The other night I decided to connect to [Untapped](https://untappd.com/) and pull down some details about Pittsburgh breweries to share as a blog post. I was really focused on sharing the universe of breweries, their locations, and most popular beers. I knew Tableau was the perfect medium – so created a visualization that showed that information. Here is the final visualization I produced and posted. I hope you find this handy and interesting!  

<iframe src="https://public.tableau.com/profile/andy.miller#!/vizhome/PittsburghBrewingScene/PittsburghCraftBrewing" height="827" width="1000"></iframe>  

[Best Viewed on Tableau Site](https://public.tableau.com/profile/andy.miller#!/vizhome/PittsburghBrewingScene/PittsburghCraftBrewing)

## The Details

For those of you interested in how I actually created this, let me give you some of the details. First, the data. Lucky for me – there is an [API for Untappd](https://untappd.com/login?go_to=https://untappd.com/api/dashboard). However, it is fairly restrictive in the amount of information that can be pulled down. They are a very small group (I think just two people), so they don’t have the resources to make their API robust and as available as they might like. Regardless, I believed the information I was looking for was there. Basically I signed up for a key, made a list of Pittsburgh breweries, created a quick Python script to extract and flatten the data, and designed a quick viz in Tableau.  

As I mentioned, the [Untapped API](https://untappd.com/login?go_to=https://untappd.com/api/dashboard) isn’t extremely robust and doesn’t allow you to search for all the breweries around a specific location, so I had to do some legwork to identify all the breweries in Pittsburgh. I used a [google sheet](https://docs.google.com/spreadsheets/d/1On718_QZkjta81yLEUpAPRt-Mx_Y8gvko-J8egy62Xc/edit?usp=sharing) to document all the breweries I could find in Pittsburgh, with the specific brewery Untappd ID (you have to use their website and check the ID in their links) – see below.

![Untappd](/psuanm5030.github.io/img/pgh_beer_02.png)

Once I had my IDs, I was good to write a few scripts that pulled down the IDs from Google Sheets, feed that to the Untappd API to request details on that brewery, which conveniently included the top 25 most popular beers, along with a bunch of metadata about the brewery (and checkins data – which I haven’t made use of yet). The Python scripts are [available on my GitHub page](https://github.com/psuanm5030/Blog/tree/master/Beer), if you are so technically inclined to check out.  

All in all, the data acquisition and viz building process was about 5-6 hours of my time – but well worth it – considering my wife (who is very supportive but doesn’t get as excited as me) was interested! I also love the convenience of this beer map!  

**The End**

Leave a comment and let me know your thoughts and if I missed any breweries!!  