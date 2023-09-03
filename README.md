# Cardiovascular_Risk_Prediction_Using_Machine_Learning
Predicting heart disease

In this notebook I will attempt to use Python libraries to create a model that predicts if a patient has heart disease.
I will take the following approach:

  1. Define the problem
  2. The data
  3. Define the evaluation metric that means success
  4. Decide which features of the given data should be focused on
  5. Create the model
  6. Experimentation with the model and data

1. Problem definition
"Given clinical parameters of a patient can the model predict whether or not they have heart disease"

As this appears to be a classification task, we will employ the Scikit-Learn algorithm to assist us in selecting the appropriate model.
https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html

2. The data
This dataset is sourced from Kaggle (https://www.kaggle.com/datasets/cherngs/heart-disease-cleveland-uci) and is originally derived from the Cleveland dataset found in the UCI ML repository. The dataset's author has made certain modifications to the descriptions.

3. Evaluation
The goal of this model is to predict whether the patients has cardiovascular disease or not.

4. Picking data features
Creating a way to easily get information about the data

Create data dictionary

age: age in years

sex: sex (1 = male; 0 = female)

cp: chest pain type
-- Value 0: typical angina
-- Value 1: atypical angina
-- Value 2: non-anginal pain
-- Value 3: asymptomatic

trestbps: resting blood pressure (in mm Hg on admission to the hospital)

chol: serum cholestoral in mg/dl

fbs: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)

restecg: resting electrocardiographic results
-- Value 0: normal
-- Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
-- Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria

thalach: maximum heart rate achieved

exang: exercise induced angina (1 = yes; 0 = no)

oldpeak = ST depression induced by exercise relative to rest

slope: the slope of the peak exercise ST segment
-- Value 0: upsloping
-- Value 1: flat
-- Value 2: downsloping

ca: number of major vessels (0-3) colored by flourosopy

thal: 0 = normal; 1 = fixed defect; 2 = reversable defect

condition: 0 = no disease, 1 = disease
