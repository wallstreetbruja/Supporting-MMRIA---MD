# Supporting-MMRIA---MD - Baltimore City 
---
title: "BMorePrentalCare"
author: "Imani Pillow"
date: "2022-10-16"
output: html_document
---

#LOAD ReadR 

```{r}
library(readr)
```


#Import Baltimore City Prenatal Dataset from 2010 - 2017 [insert citation]
```{r}
library(readr)
BMorePrenatalRates <- read_csv("Data205Project/Percent_of_Births_Where_the_Mother_Received_Early_Prenatal_Care_(First_Trimester).csv")
View(Percent_of_Births_Where_the_Mother_Received_Early_Prenatal_Care_First_Trimester_)

print(BMorePrenatalRates)
```
