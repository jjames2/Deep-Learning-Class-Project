# Deep Learning Class Project

## File Descriptions

### 1_Create_Training_Dataset

This file contains the code that transformed the data taken from Freddie Mac's "Single Family Loan-Level Dataset" into a dataset that could be used for this project. 

### 2_Engineer_Training_Dataset

Takes the dataset from 1_Create_Training_Dataset. Cleaned the dataset of missing and null values. Transformed generic "object" columns into other columns of a specific type, such as float or numeric. Columns with multiple labels were one hot encoded. Continuous data is standardized using a QuantileTransform. The new data is written to training_dat2.pkl

### training_dat2.pkl

The cleaned and standardized data to feed the model.

### scalers.pkl

Contains scalers that were used to standardize columns in training_dat2.pkl. Used to convert transformed column values back to original.

### 2_Explore

Contains visualizations of the relationships between different features in the dataset and having a loan delinquency within a year. 

### 3_Modeling_V2

Fits a deep learning model to the dataset, as well as tests the model and explains its output using SHAP.