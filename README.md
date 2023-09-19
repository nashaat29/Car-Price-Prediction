# Car Price Prediction Project

![Cover](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/bcf98373-5555-4f11-83a7-e9215caf7a97)

This project focuses on predicting car prices using Random Forest and XGBoost models. The dataset contains information on various attributes of cars, and the target variable is the price. The following sections provide an overview of the project, including dataset information, data cleaning, exploratory data analysis (EDA), and model performance evaluation.

## Dataset Information

![dataset](https://github.com/nashaat29/Car-Price-Prediction/assets/138555343/5d8ddc5f-128d-4da9-9db2-47ede2862f27)

- **Dataset Description**: The dataset consists of 19237 rows and 18 columns, including the target variable 'Price'.

### Attributes

1. ID
2. Price (Target Column)
3. Levy
4. Manufacturer
5. Model
6. Prod. year
7. Category
8. Leather interior
9. Fuel type
10. Engine volume
11. Mileage
12. Cylinders
13. Gear box type
14. Drive wheels
15. Doors
16. Wheel
17. Color
18. Airbags

Dataset Link: https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge


## Data Cleaning and Pre-processing

![after_clean](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/0083fd6d-7dde-4910-a16d-3507eb3b445e)

During the data cleaning stage, several key steps were taken to prepare the data for modeling:

1. **'Levy' Column**: Addressed the issue of '-' values.
2. **'Engine Volume' Column**: Processed turbo information.
3. **'Mileage' (km)**: Converted string values to numerical format.
4. **'Doors' Column**: Clarified the meaning of this attribute.
5. **'Wheel' Column**: Addressed different kinds of values.
6. **Dropped Columns**: 'ID' and 'Doors' were identified as useless for modeling.

The dataset was thoroughly cleaned and pre-processed to ensure quality input for the models.

## Exploratory Data Analysis (EDA)

![EDA_Dist_num](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/34db1ccd-dfd5-45ac-ab02-7797db1b276d)
![EDA_corr](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/63c600b6-968d-488f-8d51-a659291938f3)

In this stage, various aspects of the dataset were explored:

- Investigated Numerical Columns
- Plotted distributions for numeric columns
- Investigated Categorical Columns
- Examined 'Manufacturer' and 'სხვა' values
- Created countplots for categorical columns
- Explored relationships and correlations with price

## Model Performance

### Random Forest Model

![Random_res](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/27a9f42d-f440-4de1-9b81-8a101cfeb1f0)

- **R-squared**: 0.7613
- The Random Forest model explained approximately 76.13% of the variance in car prices. This indicates strong predictive capabilities.

### XGBoost Model

![XGB_res](https://github.com/nashaat29/Sales-Analysis-Dashboard/assets/138555343/9b498fa3-0769-4fb3-a278-3831a6f7fe72)

- **R-squared**: 0.7572
- The XGBoost model performed slightly below the Random Forest model, explaining about 75.72% of the variance in car prices.

Both models demonstrated strong predictive capabilities, with Random Forest showing a slightly higher R-squared value. The choice between the two models may depend on considerations such as model complexity and interpretability.

## Conclusion

In this project, significant time and effort were invested in the data cleaning and EDA stages. Both Random Forest and XGBoost models proved to be viable options for predicting car prices. Further refinement of hyperparameters and feature engineering could potentially enhance performance even further.
