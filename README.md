# Regression Models Comparison – Boston Housing Dataset

This project explores and compares different regression techniques to predict house prices using the classic Boston Housing dataset.  
The goal is to see how standard Linear Regression performs against regularized models (Ridge, Lasso) and Polynomial Regression.

## 📂 Project Overview
We train and evaluate:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **Polynomial Regression**

Each model is compared using:
- **RMSE (Root Mean Square Error)**
- **R-squared**
- **Residual analysis**

## 📊 Dataset
Boston Housing dataset contains information about housing in the Boston area, including:
- Crime rate
- Average number of rooms
- Property tax rate
- Median value of homes (target variable)

## ⚙️ Steps Performed
1. Load and explore the dataset.
2. Split into training and test sets.
3. Train Linear, Ridge, and Lasso Regression models.
4. Apply Polynomial Regression for non-linear patterns.
5. Evaluate with RMSE, R-squared, and residual plots.
6. Compare results in a summary table.

## 📈 Results
- Shows how regularization affects performance.
- Highlights situations where Polynomial Regression improves the fit.
  ## 📈 Results

| Model        | RMSE       | R-squared |
|--------------|------------|-----------|
| Linear       | 4.928602   | 0.668759  |
| Ridge        | 4.947443   | 0.666222  |
| Lasso        | 5.015535   | 0.656971  |
| Polynomial   | 3.816600   | 0.801368  |

**Insights:**
- Polynomial Regression had the best fit with the lowest RMSE and highest R-squared.
- Ridge and Lasso were very close to Linear Regression.
- Lasso slightly underperformed compared to Ridge and Linear.

### 📉 Residual Plot
Below is the residual distribution for each model.  
A good model should have residuals scattered randomly around zero, without clear patterns.

![Residual Plot](<img width="882" height="534" alt="image" src="https://github.com/user-attachments/assets/8425b7d8-3083-4e1d-978b-b320ee25203c" />)


## 🛠️ Technologies Used
- Python
- pandas
- scikit-learn
- matplotlib

## ▶️ How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/regression-models-comparison.git
