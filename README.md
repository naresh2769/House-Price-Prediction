# 🏠 Bengaluru House Price Prediction

This project aims to predict house prices in Bengaluru using a dataset of real estate listings. It includes data cleaning, feature engineering, and machine learning modeling to make accurate price predictions based on various features like BHK, square footage, and location.

---

## 📁 Dataset

- **Source**: Kaggle or other real estate data sources
- **Features**:
  - `location`
  - `size` (e.g., 2 BHK, 4 Bedroom)
  - `total_sqft`
  - `bath`
  - `price` (in lakhs)

---

## 🔍 Features Engineered

- `bhk`: Extracted number of bedrooms from `size`
- `price_per_sqft`: Computed as `price * 100000 / total_sqft`
- Cleaned `total_sqft` (handled ranges like `2100 - 2850` and other invalid formats)
- Grouped less frequent locations into a single category called **"other"**

---

## 🧹 Data Cleaning

- Dropped columns: `area_type`, `society`, `balcony`, `availability`
- Removed nulls after column drop
- Removed outliers based on:
  - Total square feet per BHK
  - Price per square foot
  - Bathrooms exceeding bedrooms by more than 2

---

## 📊 Model Building

> *(Add this section once you've implemented the model)*

- Algorithms to be tested:
  - Linear Regression
  - Lasso Regression
  - Decision Tree / Random Forest
- Evaluation Metrics:
  - RMSE, MAE, R²

---


