# Mycobacterium_Tuberculosis_Compare_Regressors
This project compares various regression models for predicting the pIC50 values of Mycobacterium tuberculosis bioactivity data using PubChem fingerprints.

## Overview
The script uses the LazyPredict library to quickly train and evaluate multiple regression models on the Mycobacterium tuberculosis bioactivity dataset. It performs the following steps:

- Load and preprocess the data
- Perform feature selection using Variance Threshold
- Split the data into training and testing sets
- Train and evaluate multiple regression models
- Visualize the results

## Usage

- Ensure you have the dataset file mycobacterium_tuberculosis_bioactivity_data_3class_pIC50_pubchem_fp.csv in the same directory as the script.
- Run the script to perform the analysis and generate visualizations.

## Key Components

- Data Loading and Preprocessing: The script loads the dataset and separates features (X) from the target variable (Y).
- Feature Selection: Variance Threshold is applied to remove low-variance features.
- Model Training and Evaluation: LazyRegressor is used to train and evaluate multiple regression models on both the training and testing sets.
- Visualization: The script generates three bar plots:

* R-Squared scores for each model
* RMSE (Root Mean Square Error) for each model
* Time taken for training each model



## Results
The script produces comparative visualizations of different regression models based on their R-Squared scores, RMSE values, and training times. These visualizations help in identifying the best-performing models for the given dataset.

![r_squared_train](https://github.com/user-attachments/assets/21a218a6-9fb4-4497-9f06-ad27273470f6)

![time_taken_train](https://github.com/user-attachments/assets/34225ea8-ddaf-469b-9fbd-e8d1e4569079)

![rmse_train](https://github.com/user-attachments/assets/7d5317c7-60de-438f-bbd6-c9ff57b1a216)


## Future Improvements

- Implement hyperparameter tuning for the best-performing models
- Add cross-validation for more robust model evaluation
- Explore feature importance and selection techniques
- Implement a prediction pipeline using the best model
