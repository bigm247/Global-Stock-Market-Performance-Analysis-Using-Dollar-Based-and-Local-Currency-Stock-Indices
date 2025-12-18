# Global-Stock-Market-Performance-Analysis-Using-Dollar-Based-and-Local-Currency-Stock-Indices

## Overview

This project analyzes global economic and financial time-series data extracted from the World Bank's Global Economic Monitor (GEM) database. The dataset includes key macroeconomic indicators such as GDP (in local currency and USD), stock market indices, and unemployment rates across countries and country groups (e.g., Advanced Economies).

The analysis follows a comprehensive econometric and machine learning pipeline to explore relationships between stock markets and macroeconomic variables, test time-series and panel data properties, and group similar economies.

## Dependencies
```bash
The attached python notebook requires the following python libraries:

- **pandas** – Data loading, manipulation, cleaning, and reshaping
- **numpy** – Numerical operations and array handling
- **matplotlib** and **seaborn** – Visualization and exploratory data analysis
- **statsmodels** – OLS regression, stationarity tests (e.g., ADF), Granger causality, cointegration tests, panel fixed effects models
- **scipy** – Supporting statistical functions
- **scikit-learn** – Data scaling (e.g., StandardScaler) and clustering (e.g., KMeans), silhouette score evaluation
- **arch** or **linearmodels** (optional, depending on implementation) – Advanced panel data models and cross-sectional dependence tests (e.g., Pesaran CD test)

Install the core dependencies with:


pip install pandas numpy matplotlib seaborn statsmodels scikit-learn 


### 1. Data Loading and Exploration
- **Initial data importation** 
- **Structural Inspection**
- **Columns Identification** 

### 2. Data Cleaning
- **Value Mapping:** Replace ".." strings with `NaN` and address missingness via imputation or deletion based on data density.
- **Tidy Transformation:** Reshaped the data from a wide format into a **long (tidy) format**, essential for panel data analysis.

### 3. Exploratory Data Analysis (EDA)
- **Summary Statistics:** Compute central tendency and dispersion for key global indicators.
- **Time-Series Visualization:** Generate line plots to track trends in GDP, stock market indices, and unemployment across decades.
- **Correlation & Distribution:** Create heatmaps to identify multi-collinearity and distribution plots to detect outliers or structural breaks in the data.

### 4. Econometric and Panel Data Tests
- **Stationarity Test:** Conducted unit root tests (e.g., **Augmented Dickey-Fuller**) to determine the integration order of the series.
- **Cointegration Test:** Evaluating long-run equilibrium relationships among non-stationary variables.
- **OLS Regression:** Estimation of baseline linear relationships between market indices and GDP.
- **Cross-Sectional Dependence:** **Pesaran’s CD test** was used to evaluate interdependence across different countries.
- **Panel Fixed Effects:** Implementation of regression models that control for unobserved country-specific heterogeneity.
- **Granger Causality:** Examining predictive causality to see if exchange rate shifts precede stock market movements.

### 5. Clustering
- **Feature Scaling:** `StandardScaler` was applied to normalize indicators with different units (e.g., percentages vs. billions of USD).
- **K-Means Clustering:** clustered countries or time periods into distinct groups based on economic performance profiles.
- **Validation:** cluster quality and separation was evaluated using the **Silhouette Score**.
```



## Aim of the project
The aim of this business data analytics project was to explore how changes in exchange rates affect how stock market performance is perceived and compared across countries. The study looked at whether stock indices measured in US dollars show different trends compared with those in local currencies and whether stable exchange rates and similar macroeconomic conditions help explain differences in market behavior between countries. This addresses a gap in existing research, which often only looks at stock markets in local currency and misses the perspective of international investors.

## Note
Check the files section for the python notebook and the datasets


