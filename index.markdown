---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignement 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

### Introduction 

This paper presents a short data story about parking safety in San Francisco, designed to assist the police reduce vehicle theft and furthermore assist drivers in making informed decisions of where to park. Using explanatory data visualizations, the paper explores the historical patterns of vehicle theft in the city and identifies areas where parking is considered safe and other areas unsafe. The explanatory analysis is divided into three sections: (1) an overview, (2) a zoomed-in analysis, and (3) a detailed examination of the data using Bokeh. In addition, the paper also evaluates the quality of the data and its impact on the outcome of the analysis.



### The Data Set

The data used in this paper is police incidents regarding vehicle thef in San Francisco in the period from 2003 to 2017 (including 2017 data). There has been 124,759 reported incidents in these 15 years. 


### Overview: Time Series Plot
To get an overview of the vehicle theft in San Francisco a time series plot is carried out to illustrate the historical behaviour of the data. The calender plot shows the number of incidents each day of the years. It is color coded with the number of incidents happening each day. A calender plot gives a detailed picture of the data and how it changes over time, giving the reader an insight into the historical data. For the vechicle theft there is a dramatical drop from one day to another in reports between 2005 and 2006. 

One could hope that this was just a sign that from one day to another San Fransisco police managed to reduce the number of vehicle incidents, but unfortunatly it looks like this is not the case and that the reason for the drop in incidents has another explanation. When looking into this drastical development it can perhaps be explained by a change in how the vechicle theft is registered in the database. This article ([link to article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report)) looks further into the subclasses under vehicle theft registrations. The article describes how San Francisco police before 2006 registered both stolen vehicles and xxx under vehicle theft whereas after 2006 it is only the stolen vehicles. This is a great example of data that can be misleading without the proper data investigation, before conclusions are made.  

 ![calplot](calplot.png)

### Zoom: Map Plot


### Details: Bokeh Plot



![bokeh](./jonatan_bokeh/assignment2_bokeh_output.html)

