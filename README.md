# 2403PTDS-RegressionBrandon
Agricultural CO₂ Emissions and Temperature Prediction
This repository contains the code, data, and analysis for predicting CO₂ emissions in the agricultural sector and assessing their impacts on temperature. Using various regression models, the project identifies the best approach for accurately predicting average temperature based on emissions data, population demographics, and other agricultural factors.

Project Overview
Context
Agriculture contributes significantly to global CO₂ emissions, which directly affects climate change. By understanding the specific sources and trends in emissions, policymakers and researchers can make informed decisions to support sustainable agricultural practices.

Problem Statement
CO₂ emissions from agricultural activities are rising, but detailed insights into major contributors and regional trends are limited. This project aims to fill that gap by:

Quantifying emissions from different agricultural sources.
Identifying emission trends across countries and over time.
Analyzing the correlation between emissions, population data, and temperature.
Objectives
Quantify Emissions: Break down emissions by agricultural activity to determine the primary sources.
Trend Analysis: Analyze historical trends in emissions data.
Correlation Assessment: Study relationships between emissions, population demographics, and temperature.
Predictive Modeling: Develop models to predict average temperature based on emission data.
Dataset
The dataset includes:

CO₂ emissions from multiple agricultural sources (e.g., forest fires, crop residues, manure management).
Population data (urban, rural, total).
Target variable: Average Temperature in °C.
Source: Provided data file co2_emissions_from_agri.csv

Methodology
Models Tested
Linear Regression
Decision Tree Regression
Random Forest Regression
Stacking Regression
Evaluation Metrics
Each model was evaluated using:

𝑅
2
R 
2
 : Measures explained variance.
Mean Squared Error (MSE): Measures average squared error in predictions.
Results
Linear Regression: 
𝑅
2
R 
2
  = 0.33, MSE = 0.205
Decision Tree Regression: 
𝑅
2
R 
2
  = 0.44, MSE = 0.171
Random Forest Regression: 
𝑅
2
R 
2
  = 0.63, MSE = 0.113
Stacking Regression: 
𝑅
2
R 
2
  = 0.63, MSE = 0.113
The Random Forest Regression model performed best, with the highest 
𝑅
2
R 
2
  and lowest MSE, making it the most suitable model for this task.

Why Random Forest?
High Predictive Power: Best balance between 
𝑅
2
R 
2
  and MSE.
Handles Complex Data: Effectively models non-linear relationships.
Stability: Less prone to overfitting than individual decision trees.
Conclusion
The Random Forest Regression model is the most reliable for predicting temperature impacts based on agricultural CO₂ emissions data. Insights from this model can guide policies toward more sustainable agricultural practices.

Getting Started
Prerequisites
Python 3.7+
Libraries: pandas, numpy, sklearn, matplotlib
