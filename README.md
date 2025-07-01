# Project Title
Aviation Accident Risk Assessment for Strategic Aircraft Acquisition

## Overview 
The objective of this project is to help a company expanding into the aviation industry identify which aircraft and operational conditions are safest. By analyzing historical accident data, we aim to minimize risk and inform aircraft purchasing decisions.

## Business Understanding
The company seeks to enter the aviation sector but lacks the necessary domain knowledge to assess risks associated with different aircraft, flight purposes, and environmental conditions. This project will uncover risk indicators and translate them into business recommendations.

Focus stakeholders:

1.  Aviation Division Head: Needs guidance on low-risk aircraft and operations.

2.  Strategic Management Team: Requires data-driven evidence for business planning.

3.  Safety & Operations Teams: Can implement the recommendations to reduce incident rates.

### Key Business Questions

1.  Which aircraft types and configurations are associated with higher accident or injury rates?

2.  Do flight purposes or weather conditions significantly affect accident severity?

3.  What data-driven recommendations can be made to reduce injury and fatality risks?


## Data Understanding and Analysis
### Data Overview

Source: Kaggle - Aviation Accident Database Synopses

File: AviationData.csv

Records: ~90,000 rows

Columns Used: 17 features after cleaning, including:

Injury_Severity, Damage_type, Flight_Purpose, Engine_Type, Fatal_Injuries, Weather, etc.

### Cleaning and Preparation

Dropped columns with more than 30% missing data

Converted injury columns to numeric

Renamed columns for clarity

Parsed Event.Date to proper datetime format

### Exploratory Data Analysis (EDA)

#### Univariate Analysis

Most aircraft in accidents were single-engine

Injury severities skewed toward fatal or serious injuries

Weather during accidents was mostly VMC (Visual Meteorological Conditions)

#### Bivariate Analysis

Personal and instructional flights had more fatal injuries than commercial ones

Accidents during VMC still resulted in high fatalities

Certain manufacturers (e.g., Cessna) appeared more frequently in the dataset

#### Multivariate Analysis

Correlation between injury counts and flight purpose/weather

Combined plots show high-risk combinations (e.g., personal flights in VMC)

#### Key Observations

Weather alone is not the best predictor of fatality risk. Most events occurred in VMC (clear weather), implying that weather isn’t always the leading factor.

Flight Purpose is a major factor: personal flights had a higher injury burden  compared to commercial or business operations.

Aircraft Make/Model patterns suggest that frequently used aircraft have more incidents, but not necessarily higher severity


## Conclusion
### Recommendations

Avoid Heavy Investment in Personal Aviation: Higher risk compared to commercial flights.

Use Weather-Insensitive Safety Protocols: High risk even in clear conditions suggests human/technical error.

Vet Aircraft by Safety Record and Engine Type: Focus on commercially proven aircraft with reliable engines.

### Project Impact

By focusing on aircraft with better safety profiles and understanding contextual risk factors, the company can make data-informed decisions that reduce liability, improve safety, and ensure a smoother entry into the aviation market.

## Tools Used
Python, Pandas, Seaborn, Matplotlib
Jupyter Notebook
Git & GitHub
Tableau Dashboard link: https://public.tableau.com/app/profile/henry.njoroge/viz/Tableau_17513224238410/Dashboard?publish=yes
