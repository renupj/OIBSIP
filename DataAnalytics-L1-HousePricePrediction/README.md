# Data Analytics L1 — House Price Prediction

## OASIS INFOBYTE — Data Analytics Internship

**Candidate:** P J Renu  
**Track:** Data Analytics  
**Task:** House Price Prediction

## Project Overview

This project builds a machine-learning regression workflow to predict house sale prices from property characteristics. It includes data cleaning, exploratory data analysis, feature preprocessing, model comparison, evaluation, and final prediction generation.

## Objectives

- Understand the factors associated with house prices.
- Perform data-quality checks and handle missing values.
- Explore price and property relationships through visualizations.
- Prepare numerical and categorical variables for machine learning.
- Compare multiple regression algorithms.
- Evaluate models using MAE, RMSE, and R².
- Generate a final house-price prediction file.

## Dataset

The included dataset is a self-contained practice dataset with realistic housing attributes and a `SalePrice` target. It is included so the project can be run without depending on an external download on submission day.

Features include:
- OverallQual
- GrLivArea
- TotalBsmtSF
- GarageCars
- BedroomAbvGr
- FullBath
- YearBuilt
- LotArea
- Neighborhood
- PropertyType

The dataset is divided into:
- `data/house_prices_train.csv`
- `data/house_prices_test.csv`

## Technology Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Machine Learning Models

The project compares:
1. Linear Regression
2. Gradient Boosting Regressor
3. Random Forest Regressor

The best model is selected automatically using the highest validation R² score.

## Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## Workflow

1. Load data
2. Inspect shape, types, duplicates, and missing values
3. Perform exploratory data analysis
4. Split features and target
5. Impute missing values
6. One-hot encode categorical variables
7. Train multiple regression models
8. Compare model performance
9. Select the best model
10. Generate predictions
11. Save model comparison and prediction outputs

## Project Structure

```text
DataAnalytics-L1-HousePricePrediction/
├── data/
│   ├── house_prices_train.csv
│   └── house_prices_test.csv
├── screenshots/
│   ├── 01_price_distribution.png
│   ├── 02_area_vs_price.png
│   ├── 03_actual_vs_predicted.png
│   └── 04_quality_vs_price.png
├── outputs/
│   ├── model_comparison.csv
│   └── house_price_predictions.csv
├── HousePricePrediction.ipynb
├── README.md
├── requirements.txt
├── DEMO_VIDEO_CHECKLIST.md
├── PROJECT_REPORT.md
└── .gitignore
```

## How to Run

Open a terminal in this project folder and install the dependencies:

```bash
pip install -r requirements.txt
```

Then start Jupyter:

```bash
jupyter notebook
```

Open `HousePricePrediction.ipynb` and run all cells from top to bottom.

## Results

The notebook automatically prints the validation MAE, RMSE, and R² score and identifies the best-performing model.

## Conclusion

This project demonstrates practical skills in data cleaning, exploratory data analysis, data preprocessing, regression modeling, model evaluation, and prediction generation.

## Submission Notes

The OASIS task workflow requires the completed project to be placed inside the single `OIBSIP` repository, with source code, a README, and relevant screenshots/output files. The project should also be demonstrated in a screen-recorded walkthrough before submission.
