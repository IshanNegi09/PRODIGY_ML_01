# House Price Prediction — Linear Regression

Predicts house sale prices from square footage, number of bedrooms, and number of bathrooms, using a linear regression model.

## Dataset

[Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

## Features used

| Feature | Column | Meaning |
|---|---|---|
| Square footage | `GrLivArea` | Above-ground living area (sq ft) |
| Bedrooms | `BedroomAbvGr` | Number of bedrooms above grade |
| Bathrooms | `TotalBath` | `FullBath` + 0.5 x `HalfBath` (engineered) |

Target: `SalePrice`

## Approach

1. Load the Kaggle House Prices dataset
2. Engineer a combined bathroom-count feature
3. Split into train/validation sets (80/20)
4. Train a scikit-learn `LinearRegression` model
5. Evaluate with R², RMSE, and MAE
6. Visualize actual vs. predicted prices
7. Generate a `submission.csv` for the Kaggle competition leaderboard

## Results

*(fill in after running the notebook: R² = ___, RMSE = $___, MAE = $___)*

## How to run

This notebook was built to run as a **Kaggle Notebook** with the competition dataset attached (in the notebook, click **+ Add Data** and search "House Prices - Advanced Regression Techniques"). It expects the files at:

```
/kaggle/input/competitions/house-prices-advanced-regression-techniques/
```

To run it elsewhere, update the two file paths in the "Load the data" cell to point to your local `train.csv` / `test.csv`, and install the packages below.

## Requirements

See `requirements.txt`.
