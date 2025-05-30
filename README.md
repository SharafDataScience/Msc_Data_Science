# Predicting COVID-19 Mortality Using Machine Learning and Regression Analysis Based on Nutrition Factors

## Project Overview

This project investigates the relationship between nutrition and the COVID-19 case fatality rate. It represents one of four key domains—Nutrition, Lifestyle & Health, Demographics, and Environmental Emissions—explored in a broader study conducted by Abdullah Sharaf under the supervision of Dr. Alma Rahat, as part of the MSc Data Science programme at Swansea University (August 2023 – October 2023).

This research project investigates the relationship between national nutrition patterns and COVID-19 mortality rates across different countries. , this project (Version 0.1 CovidAI) combines data analysis techniques with machine learning approaches using also exaplinable AI to identify significant nutritional factors that may influence COVID-19 case fatality rates.

The COVID-19 pandemic has severely impacted over 200 countries worldwide, evolving into both a major healthcare industry concern and a public health emergency. According to the World Health Organization, COVID-19 has caused over 7 million deaths globally, representing approximately 0.09% of the world's 8 billion population. This staggering figure underscores the devastating impact of the pandemic on human life and highlights the urgent need for research into factors that may influence mortality rates.

This project aims to develop robust analytical models to predict COVID-19 mortality rates using machine learning techniques, with a specific focus on nutritional factors. The findings could potentially inform public health decision-making strategies and improve the effectiveness of behavioral change interventions, particularly in educational settings.

## Repository Structure

This repository is organized into three main components:

1. Data Analysis Component (Nutrition_KG(DataAnalysis).ipynb): This notebook focuses on exploratory data analysis, statistical testing, and correlation analysis to identify significant relationships between nutritional factors and COVID-19 mortality.

2. Data Science Component (Nutrition_KG(Data_Science).ipynb): This notebook implements various machine learning models to predict COVID-19 mortality rates based on nutritional data, including feature selection, model training, and evaluation.

3. Project Presentation (Nutrition-presentation.pdf): A comprehensive presentation summarizing the project methodology, key findings, and recommendations.

## Dataset Information

The project utilizes the "COVID19 Healthy Diet Dataset" from Kaggle, which contains nutritional consumption data across different countries alongside COVID-19 case fatality rates. The dataset includes the following features:

• Country identifiers

• Consumption metrics for various food categories: Animal Products, Animal Fats, Cereals (excluding beer), Eggs, Fish & Seafood, Fruits (excluding wine), Meat, Milk (excluding butter), Miscellaneous Items, Offals, Oilcrops, Pulses, Spices, Starchy Roots, Stimulants, Sugar & Sweeteners, Treenuts, Vegetal Products, and Vegetable Oils (2020)


• Case Fatality Rate (2021) as the target variable 

## Methodology

The project methodology is divided into two main parts: Data Analysis and Data Science.

### Data Analysis Approach

The data analysis component follows a structured approach to understand the relationships between nutritional factors and COVID-19 mortality:

1. Data Loading and Exploration: Initial examination of the dataset structure, feature distributions, and basic statistics to understand the data landscape.

2. Data Wrangling: Comprehensive preprocessing including handling missing values, identifying and addressing duplicates, and managing outliers to ensure data quality.

3. Data Scaling: Standardization of features to normalize the scale differences between various nutritional metrics.

4. Exploratory Data Analysis (EDA): Visualization of distributions, relationships, and patterns in the data to gain insights into potential correlations.

5. Statistical Analysis: Application of non-parametric tests (Spearman correlation and Kendall's Tau) to identify statistically significant relationships between nutritional factors and COVID-19 mortality rates.

6. Principal Component Analysis (PCA): Dimensionality reduction to identify key factors and visualize relationships in the data through factor mapping.

### Data Science Approach

The data science component builds upon the insights from the data analysis to develop predictive models:

1. Data Preprocessing: Similar to the analysis component but with a focus on preparing data for machine learning algorithms.

2. Train-Test Split: Division of the dataset into training (80%) and testing (20%) sets to evaluate model performance on unseen data.

3. Feature Selection: Identification of the most influential nutritional factors based on statistical significance and correlation analysis.

4. Machine Learning Models: Implementation of various regression models, including:

   - Linear Regression as a baseline
     - Polynomial Regression (PL)
     - Support Vector Regression (SVR)
     - Random Forest Regression (RFR)
     - KNeighbors Regressor (KNR)
     - Gradient Boosting Regressor (GBR)
     - Multi-Layer Perceptron Regressor (MLP)

5. Explainable AI: Application of LIME (Local Interpretable Model-agnostic Explanations) to provide interpretable insights into model predictions, particularly for high and low mortality countries.

## Key Findings

The analysis revealed several significant findings regarding the relationship between nutritional factors and COVID-19 mortality:

1. Significant Correlations: The project identified statistically significant correlations between certain nutritional factors and COVID-19 case fatality rates. Specifically, higher consumption of animal products and milk (excluding butter) showed positive correlations with increased mortality rates (Spearman correlation coefficients of 0.614 and 0.644 respectively, with p-values < 0.01).

2. Negative Correlations: Conversely, higher consumption of vegetal products demonstrated a negative correlation with mortality rates (Spearman correlation coefficient of -0.614, p-value < 0.01), suggesting a potential protective effect.

3. Hypothesis Testing: Based on these findings, the null hypothesis (H₀: Nutrition does not influence COVID-19 case mortality rates) was rejected in favor of the alternative hypothesis (H₁: Nutrition influences COVID-19 case mortality rates) with a 99% confidence interval.

4. Model Performance: The Polynomial Linear Regression model demonstrated the best performance among the tested models by 0.57 R2,0.78 correlation coefficient, capturing the non-linear relationships between nutritional factors and mortality rates.

5. Explainable AI Insights: LIME analysis provided interpretable explanations for model predictions, highlighting the differential impact of nutritional factors in countries with high versus low mortality rates and show prove od data analysis key finding.


## Recommendations

Based on the project findings, the following recommendations are proposed:

1. Dietary Guidelines: Promote a balanced diet with sufficient plant-based foods to potentially reduce health risks associated with COVID-19 and similar respiratory diseases.

2. Early Intervention: Encourage behavioral change starting from an early age, particularly in primary schools, to support the development of long-term healthy eating habits.

3. Public Health Strategies: Incorporate nutritional considerations into public health decision-making strategies related to pandemic preparedness and response using polynomial regression model.

## Installation and Usage

To run the notebooks in this repository, you'll need the following dependencies:
- pip install numpy pandas matplotlib seaborn scikit-learn scipy yellowbrick plotly lime

### To use the notebooks:

1. Clone this repository

2. Ensure you have the required dependencies installed

3. Download the COVID19 Healthy Diet Dataset I provided here.

4. Run the notebooks in the following order:

   • Nutrition_KG(DataAnalysis).ipynb for exploratory analysis

   • Nutrition_KG(Data_Science).ipynb for machine learning models

## Future Work
Potential extensions and improvements for this project include:

1. Incorporating Additional Datasets:
Expanding the analysis by integrating more comprehensive datasets that contain detailed nutritional information. This would enhance the accuracy and depth of the findings.

2. Transitioning from a Cross-Sectional to a Longitudinal Study:
To move beyond correlation and better explore causal relationships, future research could adopt a longitudinal study design. By applying a multilevel modeling approach—accounting for patients nested within hospitals and regions—it would be possible to capture temporal dynamics and hierarchical structures, leading to more robust and insightful conclusions.

## References

• Kaggle COVID19 Healthy Diet Dataset ( Kaggle link: https://www.kaggle.com/datasets/mariaren/covid19-healthy-diet-dataset )

• A.Sharaf(2024) Predicting COVID-19 Mortality Using Machine Learning and Regression Analysis Based on Multiple Health- related [ResearchGate DOI](https://doi.org/10.13140/RG.2.2.27025.95844/1)

## Author

Abdullah Sharaf, under the supervision of Dr. Alma Rahat 
@ 2023-2024







