---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignment 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

## Introduction

This paper presents a short data story about parking safety in San Francisco, designed to assist the police reduce vehicle theft and furthermore assist drivers in making informed decisions of where to park. Using explanatory data visualizations, the paper explores the historical patterns of vehicle theft in the city and identifies areas where parking is considered safe and other areas unsafe. The explanatory analysis is divided into three sections: (1) an overview, (2) a zoomed-in analysis, and (3) a detailed examination of the data using Bokeh. In addition, the paper also evaluates the quality of the data and its impact on the outcome of the analysis.



### The Data Set

The data analyzed in this paper comprises police incident reports of vehicle theft in San Francisco from 2003 to 2017, including data for 2017. A total of 124,759 incidents were reported during this 15-year period.




### Overview: Time Series Plot
To get an overview of the vehicle theft in San Francisco, a time series plot is generated to visualize the historical behaviour of the data. The calender plot shows the number of incidents each day of the years, and it is color coded with the number of incidents happening each day. This type of visualization offers a detailed and informative picture of the data over time, giving readers insight into historical trends. For the vechicle theft there is a notable  drop in reports occurred between 2005 and 2006, prompting the question of whether this could be attributed to police efforts to reduce incidents. However, further investigation revealed that the drop in reported incidents was likely due to a change in how vehicle theft was registered in the police database. Prior to 2006, the police recorded both stolen vehicles and other related incidents under the category of vehicle theft. After 2006, however, only stolen vehicles were registered under this category. This example illustrates the importance of thorough data investigation before drawing conclusions, as misleading conclusions may result from incomplete or inaccurate data. For more information on this issue, see this [linked article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report).



 ![calplot](calplot.png)

### Zoom: Map Plot

<center>
<embed
       type="text/html"
       src="malou_map/heat_map.html"
       width="700"
       height="500"
       >
</center>

### Details: Bokeh Plot

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

