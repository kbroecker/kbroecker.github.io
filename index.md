---
title       : Pitch for Shiny Application
subtitle    : Conversion Calculator - Kilobytes
author      : Katherine Broecker
job         : Senior Predictive Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Overview of Project

The purpose of this project is to demonstrate a working knowledge of shiny apps by creating a simple application and publishing it to the shiny server with RStudio.  For my application I chose to create a conversion calculator that takes the user input of kilobytes and converts it to both megabytes and gigabytes.

The application can be viewed and tested at

https://kbroecker.shinyapps.io/Developing-Data-Products/

The R code used to create the shiny application is published in

https://github.com/kbroecker/Developing-Data-Products

--- .class #id 

## Conversion Refresher

Convertering data units is quite simple if one can remember the conversion amounts.  But, do we always remember?

How many Kilobytes in a Megabyte?


```r
kilobyte <- c(99, 233, 5678, 4539879)
megabyte <- kilobyte/1000
megabyte
```

```
## [1]    0.099    0.233    5.678 4539.879
```

```r
gigabyte <- kilobyte/1000000
gigabyte
```

```
## [1] 0.000099 0.000233 0.005678 4.539879
```

--- .class

## How does the shiny app work?

1. User enters in a kilobyte value with increments of 1
2. The app restates/confirms the user entry amount
3. The app outputs the converted value for megabytes and gigabytes

<div style='text-align: center;'>
  <img src='shiny_app.png' />
</div>

--- .class

## Summary

This project demonostrates that I have successfully built a simple, yet useful application using RStudio and shiny.  While the math to make the conversion from kilobytes to megabytes and gigabytes is quite simple, remembering the conversion rate may not be.  This app allows the user to quickly and easily calculate the conversion correctly every time.



