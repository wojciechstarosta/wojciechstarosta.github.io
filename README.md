---
title: "Assignment_2"
author: "Wojciech Starosta"
date: "8 paĹşdziernika 2018"
output: ioslides_presentation
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE)
```


## Agenda

Agenda

- Data summary
- Plot 1
- Plot 2

## Summary of airquality data

```{r airquality, echo = TRUE}
summary(airquality)
```

## Plotting Ozone vs Wind

```{r plot1, echo = FALSE, message = FALSE}
library(plotly)
plot_ly(airquality, x=~Ozone, y=~Wind, type="scatter")
```

## Plotting Temp vs Solar.R

```{r plot2, echo = FALSE, message = FALSE}
library(plotly)
plot_ly(airquality, x=~Temp, y=~Solar.R, type="box")
```

