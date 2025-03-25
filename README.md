# Forecasting-Sticker-Sales
This project aims to predict multiple years’ worth of sales for various Kaggle-branded stickers from different fictitious stores in different (real!) countries. Using the dataset provided in the [Playground Series - Season 5, Episode 1](https://www.kaggle.com/competitions/playground-series-s5e1/data) competition, we built and trained a predictive model that leverages advanced feature engineering and machine learning techniques.

## Project Overview

The challenge is to forecast sales (i.e., the number of stickers sold) for different date-country-store-item combinations. This synthetic dataset replicates many effects seen in real-world data, such as weekend/holiday effects and seasonality. The project details the full workflow—from data ingestion and exploratory analysis to model training and evaluation—all documented in the `sticker.ipynb` notebook.

## Dataset Description

For this challenge, you will be predicting multiple years’ worth of sales for various Kaggle-branded stickers sold by fictitious stores across real countries. Although the dataset is completely synthetic, it contains many real-world effects such as weekend and holiday effects, seasonality, etc.

### Input Features

The following columns are included in the dataset:

- **id:** Unique identifier for each sales record.
- **date:** The date of the sale.
- **country:** The country where the sale occurred.
- **store:** The name or identifier of the store.
- **product:** The specific Kaggle-branded sticker product.
- **num_sold:** The number of stickers sold on that date.

## Target Variable

- **num_sold:** Numeric variable representing the number of stickers sold, which the model aims to predict.
  
## Model Training

**Model Type:** Regression  
**Algorithm:** XG Boost  

**Training Process:**  
- The dataset was split into training and testing sets (80-20 split).  
- Preprocessing steps included handling missing values, encoding categorical variables (e.g., country, store, product), and scaling numerical features.  
- Feature engineering was applied to capture seasonal patterns, weekend/holiday effects, and other temporal trends.

**Performance:**  
The model achieved the following performance on the test set:
- **RMSE:** 170.2499
- **R-square:** 0.9394

