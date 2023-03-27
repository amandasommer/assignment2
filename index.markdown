---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

This is Assignement 2 in the course *Social Data Analysis and Visualization (02806)* offered by the *Technical University of Denmark*.

### Introduction 

This paper is a short data story about San Francisco. It investigates where it is safe to park in San Francisco to help the drivers to have a safe experience. It is an explanatory data visualization that analysis the data and aims at obtaining insight in the historical behaviour of the vehicla theft in the city. The explainatory analysis contains three parts, (1) overview, (2) zoom and filter and (3) details. The paper also evaluates the data quality and how the data influence the outcome of the analysis. (Omskriv gerne introen)



### The Data Set

The data used in this paper is police incidents regarding vehicle thef in San Francisco in the period from 2003 to 2017 (including 2017 data). There has been 124,759 reported incidents in these 15 years. 


### Time Series Plot

Initial a time series plot is carried out to illustrate the historical behaviour of the vehicle theft. Below a calender plot shows the number of incidents each day for the years. A calender plot gives a detailed picture of the data and how it changes over time providing a deeper insight into the data for the reader. For the vechical theft there is a dramatical drop in reports between 2005 and 2006. One could hope that this was just a sight that from one day to another San fransisco police managed to reduce the number of vehiclal incidents, but unfortunatly it looks like this is not the case and that the reason for the drop in incidents is due to another reason. When looking into this drastical development it can be explained by a change in how the vechical theft is registered in the database. This article ([link to article](https://www.kaggle.com/code/eyecjay/vehicle-thefts-or-jerry-rice-jubilation/report)) looks further into the subclasses under vehical theft. The article describes how San Francisco police before 2006 registered both stolen vehicals and xxx under vehicle thef whereas after 2006 it is only the stolen vehicals. This is a great example of data that can be misleading without the proper data investigation, before conclusions are made.  

 ![calplot](calplot.png)

### Map Plot


### Bokeh Plot

