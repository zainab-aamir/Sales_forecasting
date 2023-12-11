# Sales Forecasting
This repository contains a Jupyter Notebook (SalesForecasting.ipynb) focused on predicting sales using time-series data. The code is developed using Google Colaboratory.

**Dataset**

The dataset used in this project is loaded from the file train.csv. It includes information about sales, stores, items, and dates. The main objective is to predict sales based on various features.

**Data Preparation**

The notebook begins with the preparation of input data, including loading the dataset, downsampling the data for efficient processing, and converting relevant columns to appropriate data types. The dataset is split into training and testing sets based on the date.

**Feature Enrichment**

The notebook employs the upgini library for feature enrichment. It adds relevant features to the dataset, taking advantage of time-series characteristics. The CatBoostRegressor model from the catboost library is then used for training and evaluation.

**Training and Evaluation**

The model is trained in batches to handle large datasets efficiently. It is trained on the enriched features of the training data and evaluated on the corresponding enriched features of the test data. The performance is measured using the Mean Absolute Percentage Error (MAPE).

**Error Analysis**

The notebook compares the model's performance on the original dataset and the enriched dataset. The error rate (SMAPE - Symmetric Mean Absolute Percentage Error) is calculated for both cases, providing insights into the effectiveness of feature enrichment.

**Usage**
- Open the Jupyter Notebook SalesForecasting.ipynb in a compatible environment (e.g., Google Colab).
- Execute each cell sequentially to load the dataset, prepare the data, enrich features, and train/evaluate the model.
- Explore the error rates and analysis to understand the impact of feature enrichment on sales forecasting accuracy.
Feel free to experiment with different parameters, try alternative models, or customize the code to fit your specific sales forecasting needs. If using a different dataset, ensure the data format aligns with the requirements of the implemented models in this notebook.
