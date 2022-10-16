# Supporting-MMRIA---MD
---
title: "Supporting MMRIA Main"
author: "Imani Pillow"
date: "2022-10-16"
output: html_document
---

##Load Readr
```{r}
library(readr)
```


# Import MMRIA Funding and Participation Dataset
  notice the state of Maryland is funded but not a participaring state. 
```{r}
library(readr)
MMRIAData <- read_csv("data-table.csv")
View(MMRIAData)
```


