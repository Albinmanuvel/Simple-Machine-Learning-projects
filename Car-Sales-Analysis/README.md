# Car price prediction

Predicting car prices from engine and body specs. `CarPrice.csv` has 205 cars x 26 columns (no year or mileage column).

`cars.py` selects features with Welch ANOVA and Pearson correlation, then compares four regressors on a 70/30 split (`random_state=42`).

| Model | Test R2 |
|---|---|
| Linear Regression | 0.849 |
| Decision Tree | 0.872 |
| XGBoost RF | 0.919 |
| Random Forest | 0.941 |

Run: `pip install pandas numpy matplotlib scipy pingouin scikit-learn xgboost` then `python cars.py`.
