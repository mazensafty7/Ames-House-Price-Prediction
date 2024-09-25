# Ames House Price Prediction

![scatter](https://github.com/user-attachments/assets/39b7b621-4248-48a0-8f69-b31ea09302d5)

## Overview
This project predicts house prices using data from the Ames Housing Dataset. A Decision Tree model was employed to predict house prices based on various features, and the optimal parameters were determined through grid search with cross-validation. The goal of this project was to build a robust model and understand the relationships between the features and house prices.

## Project Structure
- **Data Understanding & Exploration**: Exploratory Data Analysis (EDA) was performed to identify the relationships between features and the target variable (SalePrice).
- **Data Preprocessing**: Missing and duplicated data were handled using appropriate techniques, and feature scaling was applied using Min-Max scaling. Categorical variables were transformed using one-hot encoding.
- **Modeling**: A Decision Tree model was built and tuned using grid search and 5-fold cross-validation to optimize hyperparameters.
- **Model Evaluation**: The model was evaluated on both training and test data, using metrics such as R-squared.

## Dataset
The dataset includes various features describing houses in Ames, Iowa. Some of the most important features for predicting house prices include:
- Overall Quality
- GrLivArea (Ground living area)
- GarageCars
- Year Built
- Lot Area

## Key Steps

### 1. Data Preprocessing
- **Missing Data Handling**: Missing values were imputed using the best-suited methods for each feature.
- **Feature Scaling**: A Min-Max Scaler was used to normalize the data.
- **One-Hot Encoding**: Categorical features were transformed into numerical form using one-hot encoding.

### 2. Exploratory Data Analysis (EDA)
- Visualizations and correlations were created to understand the relationships between different features and house prices.
- Important features like `Overall Quality`, `GrLivArea`, and `GarageCars` were identified as strong predictors of house prices.

<img width="574" alt="relations" src="https://github.com/user-attachments/assets/ffa7c823-46e6-4a91-8c0b-88add157fad7">

### 3. Model Building
- **Model**: Decision Tree Regressor
- **Hyperparameter Tuning**: A grid search was conducted with 5-fold cross-validation to find the optimal hyperparameters:
  - `max_depth`: 11
  - `min_samples_leaf`: 14
  - `min_samples_split`: 2

### 4. Model Evaluation
The model was evaluated on both training and test datasets using R-squared:
- **Train Score**: 0.8818
- **Test Score**: 0.8710

The relatively high scores indicate that the model performs well in predicting house prices based on the selected features.

## Conclusion
This project successfully demonstrated how a Decision Tree model can be used to predict house prices. By tuning the model's hyperparameters and handling the dataset with proper preprocessing, the model achieved a strong performance. Key insights into which features most impact house prices were gained, further enhancing model accuracy.
