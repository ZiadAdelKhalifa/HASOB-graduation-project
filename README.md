# Heart Disease Prediction Project

## Project Overview

This project aims to predict heart disease stages using a machine learning model deployed through a Flask web application. It involves data analysis, model development, and a user-friendly interface for inputting patient data and viewing predictions.

## Project Steps

### 1. Data Analysis

- **Objective:** Analyze and clean the UCI Heart Disease dataset, handling missing values efficiently.
- **Missing Values:** Instead of deleting rows (which would reduce the dataset from 920 to 299 rows), imputation with median and mode was used.
- **EDA (Exploratory Data Analysis):**
  - Used functions like `describe()`, `info()`, and `value_counts()` to understand data distribution.
  - Checked unique values in each column and explored feature relationships using plots.

### 2. Model Development

- **Model Creation:** Developed a predictive model with steps including encoding, scaling, and data splitting.
- **Performance and Saving:** The model's performance was evaluated, and the following were saved:
  - Prediction model: `heart_disease_model.keras`
  - Encoders: `heart_disease_encoder.pkl` and `heart_disease_OneHotEncoder.pkl`
  - Standard Scaler: `heart_disease_standard_scaler.pkl`
- **Integration:** Provided examples to ensure input data compatibility with the Flask app.

### 3. Flask Application

- **Purpose:** Collect inputs from users, process them, and use the model for predictions.
- **Input Consistency:** The app processes inputs using the same steps as the model development phase.

### 4. Templates

- `index.html`: A basic HTML template with input fields matching model features, a prediction button, and a section to display results.

## Saved Files

- `heart_disease_encoder.pkl` - Saved Label Encoder.
- `heart_disease_model.keras` - Saved Prediction Model.
- `heart_disease_OneHotEncoder.pkl` - Saved OneHot Encoder.
- `heart_disease_standard_scaler.pkl` - Saved Standard Scaler.
- `heart_disease_uci.csv` - Dataset in CSV format.

## Screenshots

- **Input Page (`0.png`):** Displays how users enter feature values.
- **Prediction Result (`1(1).png`):** Shows JSON output containing:
  - **Predicted Category:** The category number with the highest probability.
  - **Predicted Label:** The meaning of the predicted category.
  - **Prediction Probabilities:** Probabilities for each class in the prediction.

## How to Run the Project

### 1. Set Up the Conda Environment

Create and activate a conda environment with the required Python version:

```bash
conda create --name heart_disease_env python=3.8
conda activate heart_disease_env
