# Regression-Analysis---
title: " Predicting Sales from Advertising Spend (Linear Regression)"
author: "Your Name"
output: github_document


##  Project Description
This project analyzes the relationship between advertising spend and sales using linear regression.  
Using a dataset containing investments in TV, Radio, and Newspaper ads, the goal was to determine how strongly each channel influences sales.  
The analysis reveals that TV advertising has the most significant impact, explaining over 80% of the variation in sales.  



##  Problem Statement
Companies spend large amounts of money on advertising across multiple channels. This project explores:  

- Which advertising medium (TV, Radio, Newspaper) contributes the most to sales?  
- How accurately can we predict sales based on advertising spend?  



##  Dataset
- **Source**: `Company_data.csv` (sample dataset often used in regression problems).  
- **Features**:  
  - `TV` – Advertising budget on TV (in thousands)  
  - `Radio` – Advertising budget on Radio (in thousands)  
  - `Newspaper` – Advertising budget on Newspaper (in thousands)  
  - `Sales` – Product sales (in thousands of units)  



##  Approach
1. **Data Exploration**  
   - Shape, summary statistics, correlations, and visualizations (pairplot, heatmap).  

2. **Modeling**  
   - Built a simple linear regression model using TV as predictor.  
   - Evaluated coefficients, p-values, R², and F-statistics using `statsmodels`.  

3. **Residual Analysis**  
   - Verified assumptions of linear regression (error distribution, randomness).  

4. **Model Testing**  
   - Split dataset into train/test sets.  
   - Evaluated performance using R² score on unseen test data.  



##  Results
- TV advertising is the **most significant predictor** of Sales.  
- **Coefficient for TV**: 0.054 → every additional unit of TV spend increases Sales by ~0.054 units.  
- **R² (train)**: ~0.816 → model explains ~81.6% of variation in sales.  
- **R² (test)**: High, confirming strong predictive performance.  
- Radio and Newspaper show weaker relationships with Sales.  



##  Next Steps
- Extend to **multiple regression** using TV + Radio + Newspaper.  
- Compare model accuracy with advanced ML techniques (Ridge, Lasso, Random Forest).  
- Explore real-world datasets with larger and more diverse advertising campaigns.  

---

##  Tools & Libraries
- **Python**  
- **Pandas, NumPy** (data handling)  
- **Matplotlib, Seaborn** (visualization)  
- **Statsmodels, Scikit-learn** (modeling & evaluation)  
