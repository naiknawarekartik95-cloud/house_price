# Exploratory Data Analysis of House Prices

An enhanced exploratory data analysis (EDA) project using the **Ames Housing dataset**. The notebook studies the factors associated with house sale prices through descriptive statistics, data-quality checks and visualisations. **No machine-learning model is trained.**

**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy and Jupyter Notebook.

## Project files

```text
.
├── House_Price_EDA_Enhanced.ipynb   # Enhanced analysis notebook
├── train.csv                       # Ames Housing training dataset
├── README_Enhanced.md              # Project guide
└── (generated when notebook runs)
    ├── eda_dashboard.png
    ├── cleaned_house_prices.csv
    ├── neighbourhood_price_summary.csv
    └── saleprice_correlations.csv
```

## What the project covers

1. Dataset loading and first inspection
2. Numerical, nominal and ordinal variable classification
3. Descriptive statistics and distribution analysis
4. Correlation, covariance, scatter plots and heatmaps
5. Outlier detection using IQR and z-score methods
6. Documented missing-value handling and data-quality checks
7. Four-panel EDA dashboard
8. Verification of the original six guiding insights

## New features added

- **Quick project summary:** key dataset and sale-price statistics in one place.
- **Price per square foot:** distribution and relationship with living area and overall quality.
- **Neighbourhood comparison:** median sale prices, with a minimum sample size of 10 houses to reduce misleading comparisons.
- **Sale timing analysis:** median prices by year and month sold, alongside yearly sales counts.
- **Missing-value profile:** visual chart of missing values in the raw dataset.
- **CSV exports:** cleaned dataset, neighbourhood summary and sale-price correlation table.
- **Safer dataset loading:** the notebook checks for `train.csv` in the current working directory and reports a clear error if it is missing.

## How to run

### 1. Keep the files together

Place `House_Price_EDA_Enhanced.ipynb` and `train.csv` in the same folder.

### 2. Install the libraries

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter nbformat
```

### 3. Start Jupyter

```bash
jupyter notebook
```

Open `House_Price_EDA_Enhanced.ipynb`.

### 4. Run the notebook

Choose **Kernel → Restart & Run All**. Wait for all charts and tables to finish.

The notebook creates the CSV exports in the current working directory. The original `train.csv` is not overwritten.

## Dataset

- **Dataset:** House Prices: Advanced Regression Techniques (Ames, Iowa)
- **File:** `train.csv`
- **Rows:** 1,460
- **Columns:** 81
- **Target for descriptive analysis:** `SalePrice`
- **Source:** [Kaggle – House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

## Important interpretation notes

- This is exploratory analysis, not a house-price prediction system.
- Correlation does not prove causation.
- Price per square foot is a simple descriptive ratio, not a formal valuation.
- Neighbourhood comparisons are descriptive and can be affected by the number and mix of houses sold.
- Cleaning decisions and assumptions are documented in the notebook.
- The dataset represents sales in Ames, Iowa, so results may not generalise to other locations.

## Future improvements

- Add interactive charts with Plotly.
- Compare results before and after the documented outlier treatment.
- Add a regression model as a separate future project, with proper validation.
- Build a small web dashboard for exploring the dataset.

## Acknowledgement

Ames Housing data compiled by Dean De Cock and distributed through the Kaggle House Prices competition.
