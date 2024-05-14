# AI BOOTCAMP GROUP PROJECT (Project 1)
This repository shares the source data, examination approach, data analytics script and key findings of an examination of the impacts of extreme weather and climate events on public health and local economy, with a particular emphasis on extreme heat and impacts to North Carolina 

## Executive Summary
The three-person project team sought to examine the relationship between extreme weather and climate events across public health, agriculture, labor and other economically significant indicators.

### Summary Findings
<code style="color : name_color">[ADD SUMMARY FINDINGS HERE]</code>

### Evaluation Approach
The team sought to identify patterns, trends relationships through the evaluation of extreme weather and climate events, event-related health impacts, and the agricultural productivity and commerce trends for impacted states as well as any resulting energy system and water constraints. 
 
 To investigate the impacts, the team explored datasets published by the National Oceanic Atmospheric Agency (NOAA), Federal Emergency Management Adminstration (FEMA), US Department of Health and Human Services (HHS) and Center for Disease Control and Prevention (CDC), US Bureau of Labor Statistics (BLS), NC Department of Commerce, NC Utilities Commission, and the Federal Energy Regulatory Commission. 
 
 The team narrowed its efforts on the collection, transformation, analysis and visualization of daily, county-level data (where available) for the five-year period between 2018 - 2022, focusing on the relationship between extreme events and the following:

* _FEMA Data:_ National disaster by type, location and date declared between 2012 to 2022 period, (extracted via FEMA API)

* _US SBA Data:_ Disaster assistance issued by the US Small Business Administration (SBA) Disaster Loan Program following declared disasters occuring within the 2012 to 2022 period

* _CDC Data:_ Mortality nationwide from 2018 - 2022, including cause of death.  Certain fields (location and date of death) are redacted to protect the privacy of the decedent and families.

* _National Outbreak Reporting System (NORS)_ Reports of foodborne and waterborne disease outbreaks, as well as diseases spread by contact with environmental sources, infected people or animals.  



## Python Script Intructions
To run the associated analysis, you will need to:
* TBD
* TBD
* TBD

### Dependencies

Python Libraries
* pandas
* prophet (Google Colab)
* datetime
* numpy
* matplotlib

Datasets <code style="color : name_color">[TO BE UPDATED AND FORMATED UPON COMPLETION]</code>

* Disaster Information Dataset ( API Integration) - 2018 - 2022 
https://www.fema.gov/data-visualization/disaster-declarations-states-and-counties  - Rajesh
API Documentation # https://www.fema.gov/about/openfema/api

* Disaster Declaration Dataset 
https://lending.sba.gov/search-disaster/ - Jamie

* Disaster Loan Data - Jamie
https://data.sba.gov/dataset/e243640a-ed1c-4941-850e-b2c6aa15cad3/resource/dfca7ddd[…]a1-bb89-98fae0e6ff3a/download/sba_disaster_loan_data_fy22.xlsx

* NC Disaster
https://www.ncdps.gov/emergency-management/past-disasters

* CDC- Mike
https://data.cdc.gov
https://wonder.cdc.gov/nndss/nndss_weekly_tables_menu.asp



## Project Team Contributors
* Jamie Bond | [GitHub @JBondAI](https://github.com/jbondAI/) 
* Michael Szumski | [GitHub @mikeszumski](https://github.com/mikeszumski/)
* Rajesh Velamala | [GitHub @REJESHVELAMALA](https://github.com/rajeshvelamala/)

Other Acknowledgments
* Project instruction and requirements provided by [The Artificial Intelligence Boot Camp at UNC Charlotte](https://bootcamp.charlotte.edu/artificial-intelligence/)

