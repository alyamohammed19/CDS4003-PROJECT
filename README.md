# CDS4003-PROJECT
# Used Car Price Prediction

## Project Overview

This project aims to analyze used car data and predict vehicle prices using Data Science and Machine Learning techniques.

The project helps buyers and sellers understand how factors such as vehicle age, mileage, manufacturer, and condition relate to car prices.

### Project Objectives

- Regression: Predict used car selling prices.
- Classification: Classify cars into Low, Medium, and High price categories.
- Identify important factors that influence used car prices.

## Dataset Information

- **Dataset Name:** Craigslist Cars and Trucks Data
- **Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data
- **Original Rows:** 295,451
- **Original Columns:** 41
- **Final Prepared Rows:** 202,316
- **Final Prepared Columns:** 18

The dataset includes vehicle prices, manufacturers, models, years, mileage, conditions, fuel types, transmissions, and other vehicle information.

## Week 12 – Data Preparation Review

### 1. Data Cleaning

We performed several data cleaning tasks to improve dataset quality.

- Converted vehicle prices into numeric values.
- Removed zero, negative, and extremely high prices.
- Checked and cleaned vehicle years and odometer values.
- Investigated duplicate records using VIN numbers.
- Reduced repeated VIN listings.
- Filled missing categorical values with "Unknown".
- Selected relevant columns for further analysis.

### 2. Exploratory Data Analysis (EDA)

We created charts and performed statistical analysis to understand used car prices.

- Price Distribution
- Car Age vs. Price
- Odometer vs. Price
- Price by Manufacturer
- Price by Vehicle Condition
- Vehicle Condition Analysis
- Correlation Heatmap

**Key Findings:**

- Newer cars generally have higher prices.
- Cars with higher mileage generally have lower prices.
- Used car prices vary between manufacturers.
- Vehicle condition is associated with price differences.
- Odometer had the strongest correlation with price among the selected numerical features (-0.42).

### 3. Feature Engineering

We created three new features:

- **car_age:** Calculates vehicle age using 2026 as the reference year.
- **mileage_per_year:** Estimates average yearly mileage.
- **is_luxury:** Identifies selected luxury vehicle brands.

These features provide additional information for future Machine Learning models.

### 4. Final Data Quality Review

We checked the prepared dataset for missing values, duplicate records, and extreme prices.

The final dataset contains **202,316 rows and 18 columns**.

Some missing numerical values remain and will be handled during model training to avoid data leakage. Some matching feature rows also remain and require consideration during model evaluation.

## Tools and Libraries

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- KaggleHub
- GitHub

## Project Files

- `Data_Preparation.ipynb` – Python code, data cleaning, EDA, and feature engineering.
- `Week12_Data_Preparation_Report.docx` – Detailed documentation with code, results, and explanations.
- `README.md` – Project overview and Week 12 summary.

## Next Steps

- Prepare training and testing datasets.
- Develop regression models.
- Develop classification models.
- Evaluate and compare model performance.
- Build a Streamlit application.

## AI Assistance Disclosure

AI tools were used to assist with Python code development, explanations, documentation, and debugging. The dataset analysis and outputs were reviewed during the project.
