# brunt_calories_predictions
Brunt Calories Predictions Using ML

# Burnt Calories Prediction using Machine Learning

## Overview
This project aims to predict the number of calories burnt during exercise using various features such as gender, age, height, weight, exercise duration, heart rate, and body temperature. The dataset used for this project is a combination of two separate CSV files: `exercise.csv` and `calories.csv`.

## Dataset
The combined dataset has 15000 rows with the following columns:
- `Gender`: The gender of the user.
- `Age`: The age of the user.
- `Height`: The height of the user in centimeters.
- `Weight`: The weight of the user in kilograms.
- `Duration`: The duration of the exercise in minutes.
- `Heart_Rate`: The heart rate of the user during exercise.
- `Body_Temp`: The body temperature of the user during exercise.
- `Calories`: The number of calories burnt.

## Data Preprocessing
1. **Basic Analysis**: 
   - Checked for null values, dataset shape, and descriptive statistics using `df.info()` and `df.describe()`.
2. **Data Merging**:
   - Merged `exercise.csv` and `calories.csv` on the `User_ID` column.
   - Dropped the `User_ID` column from the combined dataframe.
3. **Data Visualization**:
   - Plotted various graphs (distplot, scatterplot, pairplot, heatmap) to understand relationships between columns.

## Model Training
Performed train-test split and used two models for training:
1. **Linear Regression**
2. **XGBRFRegressor**

## Model Evaluation
Evaluated models using:
- **Mean Squared Error (MSE)**
- **R-squared (R²) Score**
- **Accuracy Score**

### Results
- **Linear Regression**: R² Score = 0.983
- **XGBRFRegressor**: R² Score = 0.992

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/riitk/burnt_calories_prediction.git
   cd burnt_calories_prediction
