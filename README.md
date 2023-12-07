# Food Access Program Proposal Analysis

## Problem Statement

A national Medicare Advantage Plan is considering deploying a program to address food access challenges among its members and is seeking advice on the following questions: 

1) Where should the program be deployed?
2) How many people will be included? How many might be successfully engaged?
3) Which subgroup of the population might benefit the most from the program?
4) What is the projected impact of this program?

## Data Sources 
I was given two sources of data to inform my analysis: census tract-level data from the CDC and the USDA's Food Environment Atlas. I then sought out an additional dataset: a custom-built Census race and ethnicitiy dataset for the counties I selected for the program to be deployed in. I also used two papers to obtain figures that informed my projections for program engagement and impact. Below is a descipription of each source: 

**500 Cities: Census Tract-level Data**

This dataset contains information on census tracts from 500 US cities covering their populations, the prevalences of various health conditions (high cholesterol, arthritis, cancer, etc.), the prevalences of certain health behaviors (sleeping under 7 hours a night, binge drinking, smoking, etc.), and the rates of healthcare utilization (dentist visits, health insurance, Pap tests, etc.).

Link: https://chronicdata.cdc.gov/500-Cities-Places/500-Cities-Census-Tract-level-Data-GIS-Friendly-Fo/k86t-wghb

**USDA Food Environment Atlas**

This dataset was split into 4 CSV files  
* _StateAndCountyData.csv_: This dataset contains information on over 3,000 US counties covering food security, grocery store and local produce availability, socioeconomic characteristics, health and physical activity, food taxes, and food assistance program usage rates
* _SupplementalDataState.csv_: This dataset contains state population figures as well as utilization rates for a number of government food assistance programs from 2012 to 2018
* _SupplementalDataCounty.csv_: This dataset contains exact population figures from the 2010 US Census, as well as estimates for each year after until 2018
* _VariableList.csv_: This dataset contains metadata, linking the variable codes found in StateAndCountyData.csv to variable names, categories, and units of measurement

Link: https://www.ers.usda.gov/data-products/food-environment-atlas/data-access-and-documentation-downloads/

**Custom Census Race and Ethnicity Data**

This dataset contains information on the racial and ethnic makeup of the counties that I selected for the deployment of the food access program, as well as national averages. I accessed it through the advanced search feature on data.census.gov, which allowed me to customize a table to contain data on each counties' population by race (Black, White, Asian, American Indian and Alaska Native, Native Hawaiin and Other Pacific Islander, Two or More Races) and Hispanic / Latino heritage.

Link: https://data.census.gov/table?t=American%20Indian%20and%20Alaska%20Native:Asian:Black%20or%20African%20American:Hispanic%20or%20Latino:Native%20Hawaiian%20and%20Other%20Pacific%20Islander:Two%20or%20More%20Races:White&g=050XX00US06037,06065,06073

**Association between household food insecurity and annual health care costs**

This paper quantified the total annual healthcare costs for households that were food secure, marginally food insecure, moderately food insecure, and severely food insecure.

Citation: Tarasuk, V., Cheng, J., de Oliveira, C., Dachner, N., Gundersen, C., & Kurdyak, P. (2015). Association between household food insecurity and annual health care costs. CMAJ : Canadian Medical Association journal = journal de l'Association medicale canadienne, 187(14), E429–E436. https://doi.org/10.1503/cmaj.150234

**Demographic Variation in Health Insurance Coverage: United States, 2019**

This paper provided statistics for the different types of health insurance coverage for US adults by various sociodemographic characteristics. 

Link: https://www.cdc.gov/nchs/data/nhsr/nhsr159-508.pdf

## Aproach 
I determined the ideal location for a food access program based on the total number of senior residents who had low access to grocery stores in each county. I chose to focus on senior residents as most Medicare members are 65 and older, and I chose to focus on low access to grocery stores because food access largely has to do with proximity to places to purchase nutritious food. I considered focusing on the percentage of senior residents with low access to grocery stores in each county, but opted to focus on the total number to prioritize a large program reach, as choosing based on percentage shifted my recommendations toward much smaller communities where the program would be less impactful. 

Next, I calculated an estimate of how many people would be successfully engaged by the program by using four figures: the total number of senior residents with low access to grocery stores in the counties I selected; the percentage of US adults aged 65 and older who are insured through Medicare Advantage, according to the 'Demographic Variation in Health Insurance Coverage: United States, 2019" paper; the percent of the counties' eligible population who participated in SNAP (Supplemental Nutrition Assistance Program), a food assistance program that would likely be similar to this analysis's program; and the rate of increased successful member referrals to a food security organization that N1 achieved with a previous client. 

I then determined which subgroup of the population would likely benfit the most from this program by examining the racial and ethnic makeup of the selected counties compared to the national average, noting which races and ethnicities made up a larger share of the population of the chosen counties than of the nation as a whole. 

Finally, I projected the potential healthcare cost savings for the healthcare plan by referring to a paper titled 'Association between Household Food Insecurity and Annual Healthcare Costs' by Tarasuk et al. that quantified the total annual healthcare costs for households that were food secure, marginally food insecure, moderately food insecure, and severely food insecure. I made the assumption that all the senior residents with low access to grocery stores in the chosen counties fell into the marginally food insecure group (which produced the most conservative cost-saving estimate), and calculated the healthcare cost savings that would arise if we could move the same percentage of people I esimated we could engage into the food secure group. 

## Analysis
In the attached Jupyter notebook, I execute my approach and narrate along the way through Markdown comments. I begin with data collection and cleaning, then answer each question in order in separate sections. 

