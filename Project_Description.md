# Heart Disease Project_Description

## Step 1: Problem Statement
Creating a machine learning model to predict the presence of heart disease (0 = no disease, 1 = disease) using patient demographics and clinical features. The goal is to facilitate early detection and intervention for individuals at risk of heart disease.

## Step 2: Data Gathering
Collected data from Kaggle in CSV format.

## Step 3: EDA (Exploratory Data Analysis)
Performed exploratory data analysis to understand the dataset:
- Checked dataset shape: (303, 14)
- Explored dataset information and description
- Checked for null values: `df.isna().sum()`
- Identified outliers using boxenplot

## Step 4: Feature Engineering
Checked and replaced outliers using the Interquartile Range (IQR) function. The IQR method identifies data points that significantly deviate from the median. Outliers are replaced or transformed to improve model robustness.

Applied scaling using MinMaxScaler for normalization to enhance model performance. MinMaxScaler scales the data to a specific range (usually 0 to 1), preserving the relationships between data points while avoiding issues related to varying scales among features. This ensures that all features contribute equally to the model.

## Step 5: Feature Selection
Checked assumptions:
1. Linearity
2. No multicollinearity
Used train-test split to prepare the data for model training.

## Step 6: Model Training (Logistic Regression)
Applied the Logistic Regression algorithm:
- Trained the model
- Evaluated accuracy on training data: 84%
- Evaluated accuracy on testing data: 80%

## Step 7: Model Training (Random Forest Classifier)
Applied the Random Forest Classifier algorithm:
- Trained the model
- Evaluated accuracy on training data: 100%
- Evaluated accuracy on testing data: 81%
- Applied Hyperparameter Tuning:
  - Achieved accuracy on training data: 88%
  - Achieved accuracy on testing data: 82%

## Step 8: User-Defined Function
Created a user-defined function for predictions using a pickle file:
```python
import pickle

with open('heart.pkl', 'wb') as f:
    pickle.dump(hyper_model, f)

class Prediction():
    def heart_data(self, testing_data):
        with open("heart.pkl", "rb") as f:
            model = pickle.load(f)
            prediction = model.predict(testing_data)
            print("Prediction =", prediction)
        return prediction

predict = Prediction()
testing_data = x.head(50)
predict.heart_data(testing_data)
