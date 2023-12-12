# Heart Disease Prediction using Machine Learning

## About
![images](https://github.com/Yogendra-Wadkar/Heart-Disease-Prediction-using-Random-Forest-Algorithm-/assets/134367735/659ec0ba-3e30-4c10-935f-a9490da38afc)

Heart disease is a broad term encompassing various diseases and conditions affecting the heart and circulatory system. It is a major cause of disability worldwide, impacting not only the heart but also other organs and parts of the body. This project focuses on predicting the probability of a person being affected by a severe heart problem using machine learning algorithms.

## Dataset
The dataset used for this project includes the following features:

- **age:** Age in years
- **sex:** Sex (1 = male, 0 = female)
- **cp:** Chest pain type (0: typical angina, 1: atypical angina, 2: non-anginal pain, 3: asymptomatic)
- **trestbps:** Resting blood pressure (in mm Hg on admission to the hospital)
- **chol:** Serum cholesterol in mg/dl
- **fbs:** Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
- **restecg:** Resting electrocardiographic results (0: normal, 1: having ST-T wave abnormality, 2: showing probable or definite left ventricular hypertrophy)
- **thalach:** Maximum heart rate achieved
- **exang:** Exercise-induced angina (1 = yes, 0 = no)
- **oldpeak:** ST depression induced by exercise relative to rest
- **slope:** The slope of the peak exercise ST segment (0: upsloping, 1: flat, 2: downsloping)
- **ca:** Number of major vessels (0-3) colored by fluoroscopy
- **thal:** Thalassemia (0 = error, 1 = fixed defect, 2 = normal, 3 = reversible defect)
- **target (the label):** 0 = no disease, 1 = disease

## Machine Learning Algorithms
The project employs the following machine learning algorithms:

### Logistic Regression
Logistic Regression is utilized as part of the predictive modeling process. It is a statistical method for analyzing a dataset in which there are one or more independent variables that determine an outcome. In this project, it helps in understanding the relationship between various features and predicting the likelihood of heart disease.

### RandomForestClassifier
The RandomForestClassifier is employed to predict heart disease probabilities. This ensemble learning method combines multiple decision trees to create a robust and accurate model. Hyperparameter tuning has been applied to enhance the performance of the RandomForestClassifier.

## Repository Structure
- 📁 **Heart_Disease_Prediction:** Jupyter notebook detailing the entire process of heart disease prediction using machine learning.
- 📁 **Heart_Disease_Dataset:** CSV file containing the heart disease dataset used for analysis.
- 📁 **Project_Description:** Brief outline of the project's purpose and goals.

Feel free to explore the code and dataset to gain insights into the project's methodology and findings. Contributions and feedback are welcome!
