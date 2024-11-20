# Functional Data Analysis of Bike Rental Patterns

## Description
This project applies **Functional Data Analysis (FDA)** techniques to analyze rental patterns in a bike-sharing system. The study investigates hourly rentals, focusing on how factors such as temperature, season, and time of day influence demand. By leveraging FDA, continuous functions were used to identify trends, variability, and relationships that traditional time-series methods might overlook.

---

## Project Structure

### 1. Report
- **File:** `FDA Report.pdf`
- This document provides a detailed analysis of the bike rental dataset. It includes:
  - Smoothing and basis function representations.
  - Functional Principal Component Analysis (FPCA).
  - Functional Regression Analysis.
  - Functional ANOVA (FANOVA).
  - Depth Measures for outlier detection.
  - Recommendations for optimizing bike-sharing operations.

### 2. Code
- **File:** `FDA Rental Bike Sharing.Rmd`
- The R Markdown file contains all the R code used for the analysis:
  - Data preprocessing and transformation.
  - Creation of functional objects using B-splines and Fourier basis functions.
  - Regression and ANOVA models to evaluate the impact of environmental factors.
  - Depth measures and visualizations, including functional boxplots.

### 3. Data
- The analysis uses a public dataset containing hourly and daily bike rental records:
  - **Key Variables:** Date, season, weather conditions, temperature, humidity, wind speed, and rental counts.
  - **Files Needed:** Ensure the dataset (`hour.csv` and `day.csv`) is present in the working directory.

---

## Project Link
- You can access the project files and explore the analysis [here on Kaggle](https://www.kaggle.com/code/solaznog/rental-bike-sharing-dataset-eda).

---

## Key Insights
- **Hourly Demand Peaks:** High rental activity during commuting hours (morning and evening).
- **Temperature Influence:** Positive correlation between warmer temperatures and increased bike rentals.
- **Seasonal Variability:** Rentals peak in summer and fall, with lower activity in winter.
- **Weekday and Weekend Similarities:** Rental patterns are consistent across weekdays and weekends.
- **User Types:** Casual users show recreational patterns, while registered users exhibit commuting behaviors.

---

## How to Run the Project

1. **Install Required Libraries**  
   The following R libraries are used in the project:
   ```r
   library(dplyr)
   library(ggplot2)
   library(fda)
   library(fdapace)
   library(TDA)
   library(depthTools)
   library(refund)
   library(tidyverse)
   library(lubridate)
   library(splines)
   library(fda.usc)
