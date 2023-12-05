# Food Access Program Proposal Analysis

## Problem Statement

A national Medicare Advantage Plan is considering deploying a program to address food access challenges among its members and is seeking advice on the following questions: 

1) Where should the program be deployed?
2) How many people will be included? How many might be successfully engaged?
3) Which subgroup of the population might benefit the most from the program?
4) What is the projected impact of this program?

## Data Sources 
To answer these questions, I used census tract-level data from the CDC and the USDA's Food Environment Atlas. Below is a description of each source: 

**500 Cities: Census Tract-level Data**

This dataset contains information on census tracts from 500 US cities covering their populations, the prevalences of various health conditions (high cholesterol, arthritis, cancer, etc.), the prevalences of certain health behaviors (sleeping under 7 hours a night, binge drinking, smoking, etc.), and the rates of healthcare utilization (dentist visits, health insurance, Pap tests, etc.)  
Link: https://chronicdata.cdc.gov/500-Cities-Places/500-Cities-Census-Tract-level-Data-GIS-Friendly-Fo/k86t-wghb

**USDA Food Environment Atlas**

This dataset was split into 4 CSV files  
* _StateAndCountyData.csv_: This dataset contains information on over 3,000 US counties' food security, grocery store and local produce availability, socioeconomic characteristics, health and physical activity, food taxes, and food assistance program usage rates
* _SupplementalDataState.csv_: This dataset contains state population figures as well as utilization rates for a number of government food assistance programs, both from 2012 to 2018
* _SupplementalDataCounty.csv_: This dataset contains exact population figures from the 2010 US Census, as well as estimates for each year after until 2018
* _VariableList.csv_: This dataset contains metadata, linking the variable codes found in StateAndCountyData.csv to variable names, categories, and units of measurement  
Link: https://www.ers.usda.gov/data-products/food-environment-atlas/data-access-and-documentation-downloads/
