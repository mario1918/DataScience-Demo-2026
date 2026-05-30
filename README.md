# COVID-19 Data Science Analysis

A comprehensive data science project analyzing COVID-19 trends across US states using data from the New York Times, combined with demographic and political features.

## Overview

This Jupyter notebook demonstrates end-to-end data science workflow including data ingestion, exploratory data analysis (EDA), feature engineering, and visualization of COVID-19 data. The project explores correlations between COVID-19 outcomes and various state-level characteristics.

## Data Sources

1. **COVID-19 Data**: [New York Times COVID-19 Dataset](https://github.com/nytimes/covid-19-data)
   - Daily cases and deaths by US state
   - Time period: January 2020 - January 2022

2. **CDC Sugar Intake Data (2013)**: Employment-based sugar consumption statistics by state

3. **2016 Presidential Election Results**: State-level voting patterns (Democrat/Republican)

## Key Features

### Data Ingestion
- Direct CSV loading from GitHub repositories
- Date parsing and time-series indexing
- Multi-source data merging

### Exploratory Data Analysis
- Statistical summaries using `df.describe()`
- Time-series analysis with date-based filtering
- State-level comparisons and rankings
- Distribution analysis using KDE plots

### Visualizations
- **Scatter plots**: Cases vs. Deaths correlation
- **Multi-panel plots**: State-by-state linear regression analysis
- **Interactive plots**: Plotly-based time-series visualizations
- **Heatmaps**: Correlation matrices for feature relationships

### Feature Engineering
- Top 10 states by COVID-19 impact
- Political affiliation encoding (one-hot encoding)
- Combined dataset with health, political, and COVID-19 metrics

## Technologies Used

- **pandas**: Data manipulation and analysis
- **seaborn**: Statistical visualizations
- **matplotlib**: Plotting and graphics
- **plotly**: Interactive visualizations
- **Python 3.7+**

## Key Findings

The analysis explores correlations between:
- COVID-19 deaths and cases (strong positive correlation: 0.925)
- Political affiliation and COVID-19 outcomes
- Sugar intake and COVID-19 metrics
- State-level demographic factors

## Project Structure

```
.
├── Chapter7_data_science.ipynb    # Main analysis notebook
├── covid-eda.csv                   # Generated combined dataset
└── README.md                       # This file
```

## Usage

1. Open the notebook in Google Colab or Jupyter:
   ```bash
   jupyter notebook Chapter7_data_science.ipynb
   ```

2. Run cells sequentially to reproduce the analysis

3. The notebook is self-contained and fetches all data from online sources

## Notable Analyses

### Time-Series Analysis
- Date-based indexing enables efficient filtering by date ranges
- Tracks COVID-19 progression from early 2020 through 2022

### State Comparisons
- Identifies top 10 most affected states
- Creates state-specific visualizations
- Compares trends across different regions

### Multi-Feature Correlation
- Combines COVID-19 data with political and health metrics
- Generates correlation heatmaps
- Exports combined dataset for further analysis

## Book Reference

This notebook is **Chapter 7** from the book [**Minimal Python**](https://leanpub.com/minimalpython) by Noah Gift.

- [Purchase on LeanPub](https://leanpub.com/minimalpython)
- [Purchase on Amazon](https://www.amazon.com/Minimal-Python-efficient-programmer-onemillion2021-ebook/dp/B0855NSRR7)

*Licensed Under Attribution-NonCommercial-ShareAlike 4.0*

## Requirements

```
pandas
seaborn
matplotlib
plotly
jupyter
```

## Future Work

The notebook includes sections for:
- **Modeling**: Machine learning predictions (to be implemented)
- **Conclusion**: Summary of findings (to be completed)
