# FARS-dataset-visualization-report

## Introduction

Fatality Analysis Reporting System (FARS) data set is released by National Highway Traffic Safety Administration (NHTSA), and in this report the 2013-2015 accident data file is analyzed. The accident data file records the details for each traffic accident in the US that cuases death.

## View report 

Link: [EDA_1.html](https://github.com/Shiutang-Li/FARS-dataset-visualization-report/blob/master/EDA_1.html). (It should be able to be viewed in google chrome)

## Dependencies
* R version 3.3.1
* library(png)       # show images on mark down html file  
* library(grid)      # show images on mark down html file   
* library(dplyr)     # manipulate data frame  
* library(leaflet)   # interactive maps    
* library(plotly)    # pie chart   
* library(foreign)   # load .dbf file   

## Create a customized report

**Step 1. download EDA_1.rmd and set_state.png and put them into the target file folder.**  

**Step 2. download the 2013, 2014, 2015 data set from**  
ftp://ftp.nhtsa.dot.gov/fars/2013/National/FARS2013NationalDBF.zip  
ftp://ftp.nhtsa.dot.gov/fars/2014/National/FARS2014NationalDBF.zip  
ftp://ftp.nhtsa.dot.gov/fars/2015/National/FARS2015NationalCSV.zip

The link to the full description of FARS  
https://crashstats.nhtsa.dot.gov/Api/Public/Publication/812315  

**Step 3. Unzip them in the target file folder.**  

**Step 4. Use RStudio (recommended) knit html on EDA_1.rmd to create report. Make sure the required R libraries are installed.**  

**Step 5. The user could generate the report for any US state (50 states + Washington D.C.) he/she likes, by changing the "state_abbr" variable in the .rmd file**
```{r}
# Choose a state to analyze (Use Capitalized caracters!)
state_abbr <- "UT"
```
