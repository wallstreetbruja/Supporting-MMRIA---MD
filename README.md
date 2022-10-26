# Supporting-MMRIA---MD - Montgomery County 


# Import Montgomery County Hospital Maps, wrangle data, then create a map. [DATA Montgomery]

```{r}
library(readr)
DataMCHospitals<- read_csv("Hospitals_Map.csv")
View(DataMCHospitals)
```

# Import Health and Human Services Facilities 
Maternity Partnership - Prenatal Care Program
Pregnancy Testing
Fetal & Infant Mortality Review Board (FIMR or Improved Pregnancy Outcomes)
Fetal & Infant Mortality Review Board (FIMR or Improved Pregnancy Outcomes)
Nurse Case Management: Maternal and Child
```{r}
library(readr)
HHSFMC <- read_csv("Health_and_Human_Services_Facilities_List.csv")
View(HHSFMC)

## Filtering the Health and Human Services Facilities

```{r}
library(dplyr)
```

```{r}
HHSFMC1 <- HHSFMC %>%
  select(`Building Name`, `Program Name`, Zip) %>%
  filter(`Program Name` %in% c("Maternity Partnership - Prenatal Care Program", "Pregnancy Testing", "Fetal & Infant Mortality Review Board (FIMR or Improved Pregnancy Outcomes)", "Nurse Case Management: Maternal and Child", "Medical Care for Unisured Kids (Care for Kids)", "Maryland Children's Health Insurance Program (eligibility determination)"))

View(HHSFMC1)
```
