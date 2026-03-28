📌 View full report: [Live Project](https://awadhesh27.github.io/yarra-water-quality-analysis/yarra_analysis.html)
# yarra-water-quality-analysis
Exploratory data analysis of Yarra River water quality trends using R
## Overview

This project explores historical water quality data from the Yarra River (Victoria, Australia) to assess whether environmental conditions have changed over time. The analysis focuses on identifying trends in key water quality indicators between the 1990s and recent years.

## Objective

To evaluate whether water quality has declined or improved over time by analyzing key indicators such as turbidity, pH, salinity, and water temperature.

📊 Dataset
Water quality measurements across multiple years and monitoring sites
Metadata describing station characteristics
Cleaned dataset derived after preprocessing
## Key Skills Demonstrated
Data Cleaning & Preprocessing (handling missing values, filtering invalid observations)
Feature Engineering (deriving year, month, weekday, hour)
Exploratory Data Analysis (EDA)
Data Visualization using ggplot2
Statistical reasoning using null hypothesis testing and lineup methods
## Tools & Technologies
R (tidyverse, dplyr, ggplot2, lubridate)
Quarto for reproducible reporting
## Data Preparation
Removed missing or invalid datetime values
Filtered dataset to focus on observations from 1990 onwards
Derived time-based features for analysis
Excluded parameters with insufficient or non-informative data
Cleaned dataset saved for reproducibility


The final cleaned dataset contained ~1500 observations across multiple parameters and sites

## Key Insights
### Turbidity:
Decreased from the 1990s to the 2020s, suggesting potential improvement in water clarity, although variability remains due to episodic events (e.g., storms).
### pH Levels:
Increased slightly over time, indicating a shift toward more alkaline conditions.
### Water Temperature:
Increased in recent years, consistent with broader climate-related trends.
### Salinity:
Showed variability, with a decline followed by a sharp increase in recent years, suggesting changing environmental or flow conditions.
### Statistical Analysis
Applied lineup (visual inference) techniques to test hypotheses
Example:
Tested whether turbidity trends over time were statistically meaningful
Permutation-based null models suggested observed patterns were unlikely due to random variation
### Limitations
Significant data gap between 2000–2019
Some parameters not consistently measured across decades
Analysis primarily based on a single monitoring site

**These limitations restrict the ability to draw strong long-term causal conclusions**

## How to Run
Open yarra_analysis.qmd in RStudio

Install required packages:
install.packages(c("tidyverse", "lubridate", "readxl", "conflicted"))

Click Render

