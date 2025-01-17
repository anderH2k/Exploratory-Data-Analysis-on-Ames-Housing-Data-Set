# Exploratory Data Analysis (EDA) on the Ames Housing Dataset

## Objective
This project performs an exploratory data analysis (EDA) on the Ames Housing Dataset to uncover insights into the factors influencing house prices and identify relationships among various features of residential properties. The analysis includes data cleaning, descriptive statistics, univariate and bivariate analysis, and advanced visualizations.

## Dataset Information
The Ames Housing Dataset contains detailed information on residential properties in Ames, Iowa. It includes features such as the house's overall quality, lot area, neighborhood, year built, and sale price. The dataset was downloaded from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).

---

## Analysis Steps and Findings

### Step 1: Data Loading and Overview
- The dataset was loaded into a Pandas DataFrame.
- The first few rows were displayed to understand the structure of the dataset.
- A summary of the dataset was generated, including the number of rows and columns, data types, and missing values.

### Step 2: Data Cleaning
- Missing values were handled by filling numerical columns with the mean value and categorical columns with 'Unknown'.
- Duplicate rows were checked and none were found.
- Data types were converted where necessary, ensuring categorical columns were properly encoded.

### Step 3: Descriptive Statistics
- Summary statistics were computed for numerical columns such as `SalePrice`, `LotArea`, `YearBuilt`, and `OverallQual`.
- The range and distribution of the target variable (`SalePrice`) were analyzed.
- Key metrics for important features like `LotArea`, `YearBuilt`, and `OverallQual` were identified.

### Step 4: Univariate Analysis
- Histograms and KDE plots were created for numerical columns like `SalePrice`, `LotArea`, and `GrLivArea` to understand their distributions.
- Bar charts were created for categorical variables such as `Neighborhood`, `OverallQual`, and `HouseStyle` to visualize their frequency and distribution.

### Step 5: Bivariate Analysis
- The relationship between `SalePrice` and key features like `GrLivArea`, `OverallQual`, and `YearBuilt` was investigated using scatter plots and correlation coefficients.
- Box plots were created to visualize the distribution of `SalePrice` across different neighborhoods and house styles.

### Step 6: Feature Relationships and Correlations
- A correlation matrix was computed for numerical variables and visualized using a heatmap.
- The features most strongly correlated with `SalePrice` were identified and their significance was discussed.

### Step 7: Advanced Visualizations (Optional)
- Pair plots were created for selected features such as `SalePrice`, `GrLivArea`, `YearBuilt`, and `OverallQual` to visualize relationships and distributions.

---

## Key Insights
1. **Strongest Influences on `SalePrice`**:
   - `OverallQual` (Overall Quality) and `GrLivArea` (Above-Grade Living Area) have the strongest positive correlations with `SalePrice`.
   - `YearBuilt` also shows a positive correlation, indicating that newer houses tend to have higher prices.

2. **Surprising Trends**:
   - The distribution of `SalePrice` is heavily right-skewed, with a few high-end properties significantly exceeding the average price.
   - Some neighborhoods have significantly higher average prices compared to others.

3. **Potential Next Steps**:
   - Perform feature engineering to create new variables or transform existing ones.
   - Build predictive models (e.g., linear regression, random forest) to predict `SalePrice`.
   - Explore interactions between categorical and numerical features.

---

