# US-Accidents-EDA

This project involves a detailed analysis of the US Accidents Dataset to uncover insights related to traffic accidents across the United States. The dataset is sourced from Kaggle and contains information on accidents from 2016 to 2023. This analysis aims to explore various aspects of the data, including temporal trends, geographic distribution, and factors contributing to accident severity.

## Project Overview

The primary goal of this project is to analyze the US Accidents dataset to identify patterns and correlations that can help in understanding the factors influencing traffic accidents. This includes analyzing the distribution of accidents over time, identifying the most affected states and cities, and examining the impact of weather and road conditions on accident severity.

## Dataset

The dataset used in this project is sourced from Kaggle. You can download the dataset from the following link:
[US Accidents Dataset on Kaggle](https://www.kaggle.com/sobhanmoosavi/us-accidents)

## Data Wrangling

### Steps Performed:
1. **Data Cleaning:**
   - Removed unnecessary columns such as `Airport_Code`, `Wind_Chill(F)`, `Weather_Timestamp`, `Source`, and `Precipitation(in)`.
   - Dropped columns with a high percentage of missing values (`End_Lat`, `End_Lng`).
   - Converted state abbreviations to full names.
   - Handled missing values by removing rows with missing critical information and imputing mean/mode for numerical and categorical columns respectively.
   - Converted relevant columns to appropriate data types.

2. **Data Transformation:**
   - Extracted `Year`, `Month`, `Day`, and `Hour` from `Start_Time`.
   - Created a new column `Is_Weekend` to indicate if an accident occurred on a weekend.

## Exploratory Data Analysis

### Key Findings:
- **Top 10 US Cities by Accident Count:** Visualized using a pie chart, showing the proportion of accidents in the most affected cities.
- **Top 10 US States by Accident Count:** Visualized using a pie chart, highlighting California as the state with the highest accident count.
- **Temporal Analysis:** 
  - Analyzed the number of accidents per year, showing fluctuations with a peak in 2018 and a noticeable drop in 2020 due to COVID-19 lockdowns.
  - Examined monthly trends, identifying January as the month with the highest number of accidents.
  - Investigated the top weather conditions in January, noting that New Year's Day has a significant peak in accidents.

## Correlation Analysis

### Insights:
- A correlation matrix was generated to examine the relationships between different variables in the dataset.
- Significant negative correlation between temperature and humidity.
- Mild correlations between accident occurrence and traffic features such as junctions and crossings.
- Notable correlation between traffic calming measures and the presence of bumps.

## Conclusions and Recommendations

The analysis of the US Accidents dataset reveals several important insights. California stands out as the state with the highest number of accidents, necessitating targeted safety measures. The significant peak in accidents on January 1st suggests the need for increased traffic enforcement and public awareness campaigns around New Year's celebrations. The correlation analysis indicates that weather conditions and traffic features play a role in accident occurrences, highlighting the importance of weather-appropriate driving advisories and improved road infrastructure. These findings can guide policymakers, urban planners, and traffic authorities in implementing effective safety measures to reduce traffic accidents.
