# ok_obesity_analysis

# Obesity Data Analysis and Linear Regression
This repository contains Python code for analyzing obesity data and performing a linear regression analysis. The code is intended to provide insights into the relationship between various demographic factors and obesity rates in the state of Oklahoma.

## Table of Contents
- Introduction
- Data Sources
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Linear Regression Analysis
- Results Summary
### 1. Introduction
Obesity is a significant public health concern, and its prevalence can vary based on demographic factors such as age, education, gender, income, and ethnicity. This code aims to explore the relationship between these demographic factors and obesity rates in Oklahoma.

### 2. Data Sources
Two main datasets were used for this analysis:

**Demographic Data on Obesity:** This dataset contains information about obesity rates in Oklahoma based on various demographic factors, including year, state, question, percentage, age, education, gender, income, and ethnicity.

**Labels for Demographic Data:** This dataset provides descriptions for the questions in the demographic data, allowing us to replace question codes with meaningful labels.

### 3. Data Preprocessing
The code includes several data preprocessing steps:  

- Loading the data from the provided URLs into Pandas DataFrames.  
- Replacing health question codes with descriptive labels.  
- Selecting data specific to Oklahoma and obesity rates.  
- Creating separate DataFrames for each demographic factor (age, education, gender, income, ethnicity).  
- Handling missing data and dropping irrelevant rows.  
- Creating dummy variables for categorical variables.  
### 4. Exploratory Data Analysis (EDA)
The code conducts EDA to explore the relationships between demographic factors and obesity rates:

- Displaying summary information for each DataFrame.  
- Visualizing mean obesity percentages for different age groups, education levels, genders, income levels, and ethnicities using bar plots.  
### 5. Linear Regression Analysis 
The code performs a linear regression analysis to model the impact of demographic factors on obesity rates:

- Creating dummy variables for each demographic category.  
- Splitting the data into training and testing sets.  
- Training a linear regression model.  
- Making predictions on the testing set.  
- Evaluating the model's performance using Mean Squared Error (MSE).  
- Displaying the coefficients that indicate the impact of each demographic category on obesity rates.  
- Performing a statistical test on the regression model using the summary statistics.
### 6. Results Summary 
The key results from this analysis are as follows:

The linear regression model demonstrates a strong relationship between demographic factors and obesity rates in Oklahoma (R-squared: 0.866).  
Mean obesity percentages vary significantly among different demographic groups.  
Age, education, income, ethnicity, and gender all have a significant impact on obesity rates.  
For example, Asian ethnicity has the most substantial negative impact on obesity rates, while the 18-24 age group and College graduates have the most significant negative impacts.   
The categories with the most substantial positive impact on obesity rates is the age group 45 - 54 and American Indian/Alaska Native.   
The statistical test shows that the regression model is significant (p-value < 0.05), indicating that at least one of the demographic factors is associated with obesity rates. However, a white test revealed the possible presence of heteroskedasticity in the model.   
Further analysis, including a weighted regression or transforming the data, are potential areas of investigation.  
This analysis provides valuable insights for policymakers and healthcare professionals to target specific demographic groups in obesity prevention efforts.
