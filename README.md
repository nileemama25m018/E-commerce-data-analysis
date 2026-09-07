# E-commerce-data-analysis

## Overview

This project statistically analyzes an Amazon sales dataset to study how **discounts affect sales, revenue, and profit** across product categories, customer regions, and time. The analysis combines exploratory analysis, clustering, time-series analysis, and regression modeling.

## Dataset

- **50,000 orders**
- **Period:** Jan 2022 – Dec 2023
- **6 product categories**
- **4 customer regions**
- **4,000 unique products**
- Key variables: price, discount %, quantity sold, revenue, profit, rating, reviews, category, and region.

## Methodology

- **EDA:** Feature distributions, correlation analysis, and discount-level comparisons
- **Regional & Category Analysis:** Revenue and sales patterns across regions and categories
- **Clustering:** K-Means, GMM, and Hierarchical Clustering with PCA visualization
- **Product Clustering:** Grouped products based on sales and revenue
- **Time-Series Analysis:** Monthly sales, revenue, and profit trends
- **Regression:** Linear Regression, Ridge, and Lasso to analyze sales and revenue drivers

## Key Findings

- Discounts have **almost no effect on sales volume** (correlation ≈ 0.0014).
- Average revenue decreases as discount levels increase.
- Discounted orders generate lower revenue across all regions.
- Region-month clustering performs best with **K-Means at k = 2**.
- Product clustering identifies **2 major product groups** with different sales/revenue levels but similar discount patterns.
- Revenue fluctuates over time without a clear long-term trend.
- Regression models achieve approximately **R² = 0.87 for revenue**, while sales prediction gives **R² ≈ 0**.
- Overall, discounts reduce revenue and profit without generating enough additional demand to compensate for the lower selling price.

## Technologies

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `SciPy` · `Scikit-learn` · `Jupyter Notebook`

## Project Structure

```text
├── Project code_MA25M018.ipynb
├── cleaned_dataset.csv
├── README.md
└── figures/
```

## How to Run

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn
```

1. Place the dataset in the project directory.
2. Open `Project code_MA25M018.ipynb`.
3. Run all cells sequentially.

## Conclusion

The analysis suggests that **blanket discounting is not an effective strategy for increasing demand** in this dataset. Discount decisions should instead consider their impact on revenue and profit at the category, region, and product level.
