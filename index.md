---
title       : Vehicle Choice Application
subtitle    : Coursera Developing Data Products Assignment
author      : Kalai Ramea
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation

1. Transportation sector comprises about a third of greenhouse gas emissions in the US.
2. Within that, two-thirds of energy use comes from light-duty cars and trucks.
3. So, it's very important to know how the consumers make their car purchase decisions.

<div style='text-align: center;'>
    <img height='300' src='emissions.png' />
    <figcaption>Greenhouse Gas Emissions in the US (Source: EPA)</figcaption>
</div>

--- .class #id 

## 'Vehicle Choice' Shiny Application

1. This application takes in simple buyer parameters such as driving profile, attitute towards new technology, and so on to see if they can afford zero emissions cars, through a nested-logit approach (that is calculated outside of application).
2. An important part of the buyer affordability comes from infrastructure. It could be private (home / work), or it can be public (charging stations, etc.).
3. This application can give a guideline on what low emission car technology the buyer can afford over a period of 15 years (2015 to 2030).
4. It can also show how the buyer affordability can change based on basic infrastructure vs. public funded good infrastructure.

--- .class #id 

## A demo example

- Suppose if the buyer doesn't drive much (takes the car only to grocery stores), loves any new technology, and plans to buy a car in 2020 (it's a long time, but let's say he finishes his student loan then). 
- The model predicts 'Gasoline Hybrid' in a business-as-usual scenario. In this scenario government provides no subsidies for electric cars, and doesn't install any new station infrastructure.
- However, in a good infrastructure scenario, the model predicts 'electric vehicle'! In this scenario, there are a lot of public funded charging stations, which removes the range anxiety of users.

--- .class #id 

## Time series purchase trajectory over time

- The following graph is generated from the table for the buyer profile mentioned in the previous slide.It shows the top 10 technologies feasible for the buyer generated interactively from the R code.

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1.png) 
--- .class #id 




