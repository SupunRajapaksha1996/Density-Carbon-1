# **Predicting density of Carbon using Machine Learning**
## 1. Introduction
### Overview
This project explores the use of machine learning to predict the density of materials based on their properties. The dataset used is obtained from the Materials Project API, and a Linear regression model has been used for prediction.
### Objective
The goal of this project is to retrieve material properties of **Carbon** from the Materials Project API, pre-process and clean thebdata for trainign, train a machine learning model to predict density and evasluate model performance.
## 2. Dataset and Preprocessing
### Dataset source
The dataset was retrieved from the Materials Project API using *pymatgen*. The following materials properties were extracted.
+ Band Gap (eV)
+ Energy per Atom (eV)
+ Formation Energy per Atom (eV)
+ Volume (A<sup>3</sup>)
+ Bulk modulus (GPa)
+ Shear modulus (GPa)
+ Density (g/cm<sup>3</sup>)[**Target variable**]
## Data Preprocessing Steps
+ Handled missing values to replace missing data
+ Converted Dictionaries to Numeric values
+ Standardized features
+ Applied polynomial transformation
## 3. Model Training & Evaluation
### Model Selection
A Linear Regression model was trained using the preprocessed dataset. The dataset was split into
+ 80% - training set
+ 20% - test set
### Evaluation metrics
The model has been evaluated using the following metrics
+ Mean Squared Error
+ Mean Absolute Error
+ R<sup>2</sup> Score
## 4. Results
+ Mean Squared Error - 8.2369
+ Mean Absolute Error - 2.2279
+ R<sup>2</sup> Score - 0.4582
