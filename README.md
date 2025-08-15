# AI/ML Regression Playground

This notebook walks through training and evaluating four regression models—**Linear Regression**, **Ridge**, **Lasso**, and **Polynomial Regression**—on the Boston Housing dataset. The goal is to compare their performance using key metrics and visual diagnostics.

---

##  Project Overview

We explore how each model performs, with a focus on:

- **RMSE (Root Mean Square Error)** – how far off predictions are on average (in the same unit as the target).
- **R-squared** – how much of the variation in housing prices each model can explain.
- **Residual plotting** – to examine whether the model errors are randomly distributed or if there's a pattern.

---

##  Dataset

The Boston Housing dataset includes features such as:

- Crime rate
- Number of rooms per dwelling
- Property tax rate
- Median home value (the target variable)

---

##  Modeling Steps

1. **Load and explore** the dataset (basic stats, distributions).
2. **Split** into training and testing sets.
3. Train the following regression models:
   - Linear Regression  
   - Ridge Regression  
   - Lasso Regression  
   - Polynomial Regression
4. **Evaluate** each model using RMSE, R-squared, and residual plots.
5. **Compare** results in a consolidated table and visualize error patterns.

---

##  Results

| Model        | RMSE       | R-squared |
|--------------|------------|-----------|
| Linear       | 4.928602   | 0.668759  |
| Ridge        | 4.947443   | 0.666222  |
| Lasso        | 5.015535   | 0.656971  |
| Polynomial   | 3.816600   | 0.801368  |

**Key insights:**
- **Polynomial Regression** clearly outperformed the other models — lower RMSE and higher R-squared indicate it captured the data pattern more effectively.
- **Ridge** and **Lasso** performed similarly to Linear Regression, with only minor differences.
- **Lasso** slightly underperformed compared to Ridge and Linear in this dataset context.

---

###  Residual Plot

Below is the residual distribution for each model, showing how errors vary across predicted values. A well-behaved model shows errors scattered around zero, without systematic patterns.

![Residual Plot](residual_plot.png)

---

##  Technologies Used

- Python  
- pandas  
- scikit-learn  
- matplotlib  

---

##  Getting Started

```bash
git clone https://github.com/Adeel-Gill/ai-ml-regression-playground.git
cd ai-ml-regression-playground
pip install -r requirements.txt
jupyter notebook house-price-prediction-regression.ipynb
