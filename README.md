🦠 Predicting COVID-19 Mortality Using Machine Learning and Regression Analysis Based on Nutrition Factors
This repository contains the research project titled "Predicting COVID-19 Mortality Using Machine Learning and Regression Analysis Based on Nutrition Factors" , developed by Abdullah Sharaf under the supervision of Dr. Alma Rahat (Version 0.1 - CovidAI ).

The project explores how national nutrition patterns may influence COVID-19 mortality rates across different countries using a combination of statistical analysis, machine learning models, and explainable AI techniques.

🧭 Project Overview
The global impact of the COVID-19 pandemic has been immense, with over 7 million deaths reported globally as of 2023. This project investigates whether nutritional factors at the country level are associated with variations in case fatality rates .

We apply exploratory data analysis , machine learning regression models , and interpretability tools (LIME) to analyze and predict mortality based on dietary consumption patterns.

📁 Repository Structure
The repository is organized into three main components:

Data Analysis Notebook : Nutrition_KG(DataAnalysis).ipynb
Exploratory Data Analysis (EDA)
Statistical testing
Correlation analysis
Data Science Notebook : Nutrition_KG(Data_Science).ipynb
Feature selection
Model training and evaluation
Explainable AI (LIME)
Project Presentation : Nutrition-presentation.pdf
Summary of methodology, findings, and recommendations
📊 Dataset Information
The dataset used is the COVID19 Healthy Diet Dataset from Kaggle, containing:

Country identifiers
Nutritional consumption metrics across multiple food categories:
Animal Products, Cereals, Eggs, Fish & Seafood, Fruits, Meat, Milk, Pulses, Vegetable Oils, etc.
Target variable: Case Fatality Rate (2021)
🔍 Methodology
📈 Data Analysis Approach
Data Loading & Exploration
Data Wrangling (missing values, duplicates, outliers)
Data Scaling
Exploratory Data Analysis (EDA)
Statistical Testing (Spearman, Kendall’s Tau)
Principal Component Analysis (PCA)
🤖 Data Science Approach
Data Preprocessing
Train-Test Split (80-20)
Feature Selection
Machine Learning Models Tested :
Linear Regression
Polynomial Regression
Additional tuned regression models
Explainable AI (LIME) for model interpretation
📌 Key Findings
✅ Positive correlations between mortality and consumption of:
Animal products (ρ = 0.614)
Milk (excluding butter) (ρ = 0.644)
❌ Negative correlation observed with:
Vegetal products (ρ = -0.614)
🧪 Hypothesis testing rejected the null hypothesis:
H₀: Nutrition does not influence mortality
H₁: Nutrition influences mortality (p < 0.01, 99% confidence)
📉 Best performing model: Polynomial Regression
💡 LIME insights showed interpretable differences in nutritional impact across high- and low-mortality countries
📢 Recommendations
Promote plant-based diets as part of public health strategies
Encourage early education on healthy eating habits
Integrate nutrition planning into pandemic preparedness policies
⚙️ Installation & Usage
Dependencies
Install required packages using pip:

bash


1
pip install numpy pandas matplotlib seaborn scikit-learn scipy yellowbrick plotly lime
Steps to Run
Clone the repo:
bash


1
git clone https://github.com/yourusername/covid19-nutrition-ml.git 
Install dependencies
Download the dataset from Kaggle
Run notebooks in order:
Nutrition_KG(DataAnalysis).ipynb
Nutrition_KG(Data_Science).ipynb
🔮 Future Work
Potential extensions include:

Adding more detailed nutritional datasets
Incorporating time-series dietary changes
Investigating demographic and regional variations
Applying ensemble and deep learning methods
Expanding analysis to other health outcomes
📚 References
World Health Organization (WHO) – COVID-19 Statistics
Kaggle Dataset: COVID19 Healthy Diet Dataset
Statistical Methods: Spearman, Kendall’s Tau, PCA
ML Techniques: Linear & Polynomial Regression, LIME
