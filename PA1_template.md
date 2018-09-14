---
title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---
###**Author**: Ankit Singhal
###**Date**  : 14-Sep-2018

## **Part1: Loading and preprocessing the data**
'''{r echo=FALSE}  
setwd("C:\\Machine Learning\\RepData_PeerAssessment1")  
mydf <- read.csv(unz("activity.zip", "activity.csv"))  
sapply(mydf, class)  
'''  
activity$date is converted from factor to date class. I used the "zoo" package to manage the time serie which, furthermore, is regularly spaced. The data are collected on 61 days.  
'''{r}
activity$date <- as.Date(activity$date, format = "%Y-%m-%d")
suppressWarnings(library(zoo))
'''
## **Part2: What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
