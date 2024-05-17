 # AI BOOTCAMP GROUP PROJECT (Project 1)
This repository shares the source data, examination approach, data analytics script and key findings of an examination of the impacts of disasters and extreme weather events on US public health and economics.

## EXECUTIVE SUMMARY

### Project Objectives
To examine the impacts of extreme weather and climate events on public health and regional  economics. 

### Data Analysis
The investigating team narrowed its efforts on the collection, transformation, analysis and visualization of daily, county-level data, where available, for at least five years including the period between 2018 - 2022, and focusing on the relationship between extreme events. 

We conducted data discovery activites to sharpen our focus on datasets made available by FEMA (disaster data) and CDC (public health data). Using Python tools and libraries, the investigating team conducted the following key activities:
* Data Identification and Exploration –  identified and reviewed available datasets, screening for data applicability and data quality
* Data Transformation – imported, cleaned and joined datasets by location and date attributes or disaster ID
* Data Analysis – explored the relationship of the various datasets  

### Summary Findings
Analyses revealed little relationship between declared disasters public health data with possible exception of hospitalization counts and the 2020 COVID-19 disaster declaration in Texas.
The investigating team did identify data suggesting that disaster declarations are becoming more frequent nationwide which suggests that disaster recovery costs will also continue to rise.


## ANLYSIS DETAILS
Across the US, major weather and climate events appear to be occurring more frequently and with greater intensity. Consequently, we expected to find observable impacts to the health, safety and economic data reported across the country and sought to identify patterns, trends and/or relationships through the evaluation of disaster and public health datasets. 
 
To investigate the impacts, the team explored datasets published by the National Oceanic Atmospheric Agency (NOAA), Federal Emergency Management Adminstration (FEMA), US Department of Health and Human Services (HHS) and Center for Disease Control and Prevention (CDC), US Bureau of Labor Statistics (BLS), NC Department of Commerce, NC Utilities Commission, and the Federal Energy Regulatory Commission. 

### Datasets Analyzed
The team narrowed its efforts on the collection, transformation, analysis and visualization of daily, county-level data (where available) for the five-year period between 2018 - 2022, focusing on the relationship between extreme events and the following:

__FEMA Datasets__ (extracted via APIs)
* [Disaster Declaration Summaries for State and Counties (1953 to 2023)](https://www.fema.gov/data-visualization/disaster-declarations-states-and-counties)
* [Public Assistance Funded Projects (1998 - 2023)](https://www.fema.gov/openfema-data-page/public-assistance-funded-projects-details-v1)

__Nationa CDC Datasets__ (ingested datasets downlated from CDC data library)
* [National Outbreak Reporting (2010 to 2022)](https://wonder.cdc.gov/nndss/nndss_weekly_tables_menu.asp)
* [Mortality Data for Public Use (2018 to 2023)](https://www.cdc.gov/nchs/nvss/mortality_public_use_data.htm)


### Data Analysis Using Python
The team developed the __USDisaster_and_PublicHealth_DataAnalysis.ipynb__ python notebook to ingest, explore, transform, visualize and merge the datasets. Once merged, the investigating team analyzed a dataframe consisting for 430,142 records with 9 attributes:
* Disaster number
* Disaster name
* Project Amount
* Year
* Month
* State 
* Hospitalizations
* Illnesses
* Deaths

Within the notebook, the investigating team analyzed the relationships between several attributes to determine if relationships between disaster declarations and public health could be detected. Using the dollar amounts awarded for disaster recovery projects as a measure of disaster cost, the team investigated relationships between disaster declarations and the following:
* Public Assistance Project Amounts (billions USD)
* US Deaths
* Hospitalizations
* Reported Illnesses

### Analysis Results
__Key Observations__ 
* Texas observed to be a clear outlier for number of disaster declarations
* 2017 disaster declaration in Puerto Rico (Hurricanes Irma and Maria) and 2020 disaster declarations in TX and NY (COVID-19) three of the highest publicly funded disasters in US history 
* Proliferation of privacy protection rules resulted in low resolution public health data being made available for public use (i.e., data not reported by location), dampening its utility for this analysis.

__Key Analysis Findings__
* 2017 Hurricane Irma/Maria disaster declaration in Puerto Rico corresponded with the highest disaster assistance funding in our dataset 
* 2019 winter storm disaster declaration in Oregon corresponded with the highest US death counts in our dataset 
* 2020 COVID-19 disaster declaration in Texas corresponded with the highest hospitalization count in our dataset
* 2018 Hurricane Micheal disaster declaration in Florida corresponded with the highest illness count in our dataset

### Conclusion
While it may be likely that the 2020 COVID-19 disaster declaration in Texas and peak hospitalization counts are related, the investigating team saw no compelling evidence to suggest a meaningful relationship between the peak death and illness counts the concurrent disaster declarations identified

Given access to higher fidelity public health data and additional time to explore more public data, the investigating team may have opted to explore the following areas:
* Evaluation of state-level disaster data normalized by land area and per capita
* Relationship between extreme heat events (historically excluded from disaster declarations) on mortality and agricultural and productivity losses
* Relationship between major flood events and prevalence of mosquito born illnesses
* Possibility of a delayed relationship between public health data and disaster declarations



## ADDITIONAL REFERENCE CONTENT
### Python Libraries
* datetime
* json
* math
* matplotlib
* numpy
* pandas
* request
* seaborn

### Project Contributors
* Jamie Bond | [GitHub @JBondAI](https://github.com/jbondAI/) 
* Michael Szumski | [GitHub @mikeszumski](https://github.com/mikeszumski/)
* Rajesh Velamala | [GitHub @REJESHVELAMALA](https://github.com/rajeshvelamala/)

## Other Acknowledgments
* Project instruction and requirements provided by [The Artificial Intelligence Boot Camp at UNC Charlotte](https://bootcamp.charlotte.edu/artificial-intelligence/)

