---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignement 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

### Introduction 

This paper presents a short data story about parking safety in San Francisco, designed to assist the police reduce vehicle theft and furthermore assist drivers in making informed decisions of where to park. Using explanatory data visualizations, the paper explores the historical patterns of vehicle theft in the city and identifies areas where parking is considered safe and other areas unsafe. The explanatory analysis is divided into three sections: (1) an overview, (2) a zoomed-in analysis, and (3) a detailed examination of the data using Bokeh. In addition, the paper also evaluates the quality of the data and its impact on the outcome of the analysis.



### The Data Set

The data analyzed in this paper comprises police incident reports of vehicle theft in San Francisco from 2003 to 2017, including data for 2017. A total of 124,759 incidents were reported during this 15-year period.




### Overview: Time Series Plot
To get an overview of the vehicle theft in San Francisco, a time series plot is generated to visualize the historical behaviour of the data. The calender plot shows the number of incidents each day of the years, and it is color coded with the number of incidents happening each day. This type of visualization offers a detailed and informative picture of the data over time, giving readers insight into historical trends. For the vechicle theft there is a notable  drop in reports occurred between 2005 and 2006, prompting the question of whether this could be attributed to police efforts to reduce incidents. However, further investigation revealed that the drop in reported incidents was likely due to a change in how vehicle theft was registered in the police database. Prior to 2006, the police recorded both stolen vehicles and other related incidents under the category of vehicle theft. After 2006, however, only stolen vehicles were registered under this category. This example illustrates the importance of thorough data investigation before drawing conclusions, as misleading conclusions may result from incomplete or inaccurate data. For more information on this issue, see this [linked article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report).



 ![calplot](calplot.png)

### Zoom: Map Plot


### Details: Bokeh Plot



![bokeh](./jonatan_bokeh/assignment2_bokeh_output.html)

