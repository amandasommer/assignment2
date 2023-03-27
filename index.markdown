---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignment 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

## Introduction

This paper presents a short data story about parking safety in San Francisco, designed to assist the police reduce vehicle theft and furthermore assist drivers in making informed decisions of where to park. Using explanatory data visualizations, the paper explores the historical patterns of vehicle theft in the city and identifies areas where parking is considered safe and other areas unsafe. The explanatory analysis is divided into three sections: (1) an overview, (2) a zoomed-in analysis, and (3) a detailed examination of the data using Bokeh. In addition, the paper also evaluates the quality of the data and its impact on the outcome of the analysis.



## The Data Set

The data analyzed in this paper comprises police incident reports of vehicle theft in San Francisco from 2003 to 2017, including data for 2017. A total of 124,759 incidents were reported during this 15-year period.




## Overview: Time Series Plot
To get an overview of the vehicle theft in San Francisco, a time series plot is generated to visualize the historical behaviour of the data. The calender plot shows the number of incidents each day of the years, and it is color coded with the number of incidents happening each day. This type of visualization offers a detailed and informative picture of the data over time, giving readers insight into historical trends. For the vechicle theft there is a notable  drop in reports occurred between 2005 and 2006, prompting the question of whether this could be attributed to police efforts to reduce incidents. However, further investigation revealed that the drop in reported incidents was likely due to a change in how vehicle theft was registered in the police database. Prior to 2006, the police recorded both stolen vehicles and other related incidents under the category of vehicle theft. After 2006, however, only stolen vehicles were registered under this category. This example illustrates the importance of thorough data investigation before drawing conclusions, as misleading conclusions may result from incomplete or inaccurate data. For more information on this issue, see this [linked article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report).





 ![calplot](calplot.png)
 
 When looking at the rest of the calender plot, the number of incidents is more or less evenly destributed over the years. Some peak are happening, but it does not seems like any events has triggered these peaks. The plot shows that there are very few vehicle theft in 2010 and July 2011 than the other years and more in 2015. 

## Zoom: Map Plot
If you're planning to visit San Francisco and are wondering where it's safe to park your car, it's worth exploring the data on vehicle thefts in the city. According to [an article](https://www.nbcbayarea.com/investigations/breaking-point-sf-suffers-highest-rate-of-car-break-ins-compared-to-atlanta-dc-dallas-la/2731757/) from 2016, many tourist areas in San Francisco have a high number of vehicle thefts, as do certain parking lots and areas close to highways. 

To visualize this data, we created a heat map showing the locations of both tourist attractions (marked in purple) and parking lots (marked in orange). We also included major freeways and highways in San Francisco (marked in red) for reference. By clicking on the markers, you can see the names of the tourist attractions or parking lots. The map shows vehicle thefts from one week in August 2016.

The map shows that certain areas with many tourist attractions or parking lots are more prone to vehicle thefts, but there are also many areas where this is not the case. The same goes for the areas around highways. The east side highways have a lot of vehicle thefts in the surrounding areas, whereas the west side does not seem to have this issue.

It's important to note that the visualization is based on a limited dataset, and not all tourist attractions or parking lots are included on the map, which limits the conclusions we can draw. However, the map opens up opportunities for further exploration.

What we can see from the map is that the east side of San Francisco had significantly more vehicle thefts during the specific week that we analyzed. So, if you're planning to park your car in San Francisco, it might be worth considering whether you're parking it close to a tourist attraction, a big public parking lot, or a highway, as these areas may be at a higher risk of vehicle theft!

<center>
<embed
       type="text/html"
       src="malou_map/heat_map.html"
       width="700"
       height="500"
       >
</center>

## Details: Bokeh Plot

The following Bokeh visualization is an interactive line graph that shows the evolution of car thefts from 2008-2017 for each SF district. As of 2017, Bayview, Mission and Southern receives the most reports of vehicle theft, with 1 report for every 100 citizens each year! However, it should be noted that there isn't a one-to-one correlation between the population size of a district and the number of cars parked within it – this should be taken into consideration when interpreting the data.

One thing that stands out when observing the evolution of vehicle thefts across the 10 year period is a spike in reported vehicle crimes in 2015 and a dip in vehicle theft in 2010. These variations in the data is (for the most part) city-wide, which hints at the fact that temporal variations in crime happens on a city-wide level rather than at district scale. The data does not offer a clear explanation for these variations. When evaluating the overall trajectory of vehicle thefts, there doesn't seem to be a clear upwards or downwards trajectory (due to the yearly variance, a 10-year time period is too small of a timescale for this kind of analysis). The crime ranking of each districts in comparison to each other is stable as well, showing that it's the same disctricts that are struggling with vehicle crimes year after year.

The police districts have widely different population sizes, with the smallest district (Tenderlion) only having a population of ~36,000 citizens compared to Taraval's population size of ~155,000 citizens. [[Source: prisonpolicy.org]](https://www.prisonpolicy.org/origin/ca/2020/sanfrancisco_police.html). Because of this, the data has been adjusted to list the number of reports per 100,000 capita. If left unadjusted, the smaller districts would appear to be disproportionally safe as a place to park compared to the bigger districts.

In conclusion, this graph shows that Tenderloin and Taraval is the safest districts to park vehicles, and that this has been an ongoing trend across several years.

<center>
<embed
       type="text/html"
       src="assignment2_bokeh_output.html"
       width="700"
       height="500"
       >
 </center>

