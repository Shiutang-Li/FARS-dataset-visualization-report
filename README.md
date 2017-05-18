# FARS-dataset-visualization-report

Fatality Analysis Reporting System (FARS) data set is released by National Highway Traffic Safety Administration (NHTSA), and in this report the 2013-2015 accident data file of it is analzyed. The accident data file records the details for each traffic accident in the US that cuases death.

1. To view the visulization report with interactive maps, download EDA_1.html.

2. To create a customized report:

**Step 1. download EDA_1.rmd and set_state.png and put them into the target file folder.**  

**Step 2. download the 2013, 2014, 2015 data set from**  
ftp://ftp.nhtsa.dot.gov/fars/2013/National/FARS2013NationalDBF.zip  
ftp://ftp.nhtsa.dot.gov/fars/2014/National/FARS2014NationalDBF.zip  
ftp://ftp.nhtsa.dot.gov/fars/2015/National/FARS2015NationalCSV.zip

**Step 3. Unzip them in the target file folder.**  

**Step 4. Use RStudio (recommended) knit html on EDA_1.rmd to create report. Make sure the following R libraries are installed:**  

library(png)       # show images on rmd  
library(grid)      # show images on rmd  
library(dplyr)  
library(leaflet)   # for interactive maps  
library(plotly)    # for pie chart  
library(foreign)   # to load .dbf file  

**Step 5. The user could generate the report for any US state (50 states + Washington D.C.) he/she likes, by changing state_abbr in the .rmd file**
```{r}
# Choose a state to analyze (Use Capitalized caracters!)
state_abbr <- "UT"
```
