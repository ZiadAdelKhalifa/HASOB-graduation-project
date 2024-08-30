Project Overview
This project focuses on predicting heart disease using the UCI Heart Disease dataset. The process involves data analysis, model building, and deploying a Flask application to make predictions based on user inputs. Below are the detailed steps of the project:

Steps of the Project:
1. Data Analysis
Dataset: UCI Heart Disease Data.
Data Cleaning: Managed null values by considering alternatives like median and mode imputation instead of deletion, preserving the dataset size from reducing to 299 rows out of 920.
Exploratory Data Analysis: Used functions such as describe(), info(), and value_counts() to understand the data. Analyzed relationships between features and visualized the data using plots for individual columns, as well as pairwise comparisons.
2. Model Building
Preprocessing: Performed data cleaning, encoding (OneHotEncoder and LabelEncoder), and scaling (StandardScaler). The data was then split into training and testing sets.
Model Development: Built a prediction model and evaluated its performance.
Saving Components: Saved the trained model, encoders, and scaler for future use.
Example Usage: Provided an example of how to process inputs to be compatible with the model, which was useful in developing the Flask application for real-time predictions.
3. Flask Application
Functionality: Developed a Flask app to accept inputs from patients or doctors, process them, and use the trained model to predict heart disease. The input processing steps align with those used in the model development notebook.
4. Templates
Index Page: The app includes a basic HTML page (index.html) with input fields for model features and a button to trigger predictions. It displays the prediction results clearly to the user.
Saved Files
heart_disease_encoder.pkl: Saved Label Encoder.
heart_disease_model.keras: Saved prediction model.
heart_disease_OneHotEncoder.pkl: Saved OneHot Encoder.
heart_disease_standard_scaler.pkl: Saved Standard Scaler.
heart_disease_uci.csv: CSV file containing the dataset.
