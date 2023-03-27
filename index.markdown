---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignement 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

### Introduction 

This paper is a short data story about San Francisco. It investigates where it is safe to park in San Francisco, in order to help the drivers have a safe experience. It is an explanatory data visualization that analysis the data and aims at providing meaningfull insight in the historical behaviour of the vehicle theft in the city. The explainatory analysis consist of three parts; (1) overview, (2) zoom and (3) details. The paper also evaluates the data quality and how the data influence the outcome of the analysis. 



### The Data Set

The data used in this paper is police incidents regarding vehicle thef in San Francisco in the period from 2003 to 2017 (including 2017 data). There has been 124,759 reported incidents in these 15 years. 


### Overview: Time Series Plot
To get an overview of the vehicle theft in San Francisco a time series plot is carried out to illustrate the historical behaviour of the data. The calender plot shows the number of incidents each day of the years. It is color coded with the number of incidents happening each day. A calender plot gives a detailed picture of the data and how it changes over time, giving the reader an insight into the historical data. For the vechicle theft there is a dramatical drop from one day to another in reports between 2005 and 2006. 

One could hope that this was just a sign that from one day to another San Fransisco police managed to reduce the number of vehicle incidents, but unfortunatly it looks like this is not the case and that the reason for the drop in incidents has another explanation. When looking into this drastical development it can perhaps be explained by a change in how the vechicle theft is registered in the database. This article ([link to article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report)) looks further into the subclasses under vehicle theft registrations. The article describes how San Francisco police before 2006 registered both stolen vehicles and xxx under vehicle theft whereas after 2006 it is only the stolen vehicles. This is a great example of data that can be misleading without the proper data investigation, before conclusions are made.  

 ![calplot](calplot.png)

### Zoom: Map Plot


### Details: Bokeh Plot



![bokeh](./jonatan_bokeh/assignment2_bokeh_output.html)

