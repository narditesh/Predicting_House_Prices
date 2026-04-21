# 🏡 Predicting House Prices
This project builds and evaluates machine learning models (Linear Regression, Ridge, and LASSO) to predict house prices using various property features.
# 📌 Overview

This project builds and evaluates machine learning models Linear Regression, Ridge Regression, and LASSO Regression to predict house prices based on different property features.
The goal is to understand feature relationships, improve model performance, and compare regularized models.

# 📊 Dataset

The dataset contains numerical features related to houses (e.g., Lot Size, bedrooms, house Age, etc.) and the target variable House_Price.

# 🔍 Key steps performed

Data inspection using df.info(), df.describe(), and shape analysis

Correlation analysis

Heatmap visualization

Train–test split

Model training and evaluation

Regularization (Ridge & LASSO)

Saving the best model using joblib

# 🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib / Seaborn

scikit-learn

statsmodels

Joblib

# 🤖 Model Training

Models implemented:

Linear Regression

Ridge Regression

LASSO Regression

# 📏 Evaluation metrics

R² Score

MSE

RMSE

# 📊 Results

Both Ridge Regression and LASSO Regression produced very similar results when predicting house prices. The performance comparison is shown below:

| Model | Train R² | Test R²|
|-------|----------|--------|
| LASSO | 0.6937   | 0.5335 |
| Ridge | 0.6936   | 0.5337 |


# 🔍 Interpretation

The models explain about 53% of the variation in house prices a moderate level of predictive power.

Ridge Regression performed slightly better on the test data, but the difference is very small.

Train and test scores are close, which shows the model is not overfitting.

Regularization (Ridge/LASSO) did not significantly change performance, meaning the dataset is fairly stable.

# ▶️ How to Run

1. Open the notebook in Google Colab:
   [house_prices_portfolio.ipynb](https://colab.research.google.com/github/narditesh/Predicting_House_Prices/blob/main/house_prices_portfolio.ipynb)
   
2.  If running locally, clone the repository:  
   git clone https://github.com/narditesh/Predicting_House_Prices.git    

# ✔️ Conclusion

Ridge is chosen as the final model because of its slightly higher test score and smoother coefficient behavior. The trained Ridge model is saved using joblib for future use.
