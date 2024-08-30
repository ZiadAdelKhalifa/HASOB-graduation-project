<h1>Steps of the project :</h1>

<h2>1- Data Analysis :</h2>
<h4>
  - Analysis of the UCI Heart Disease Data, focusing on data cleaning to handle null values. <br>
  - Instead of deleting null values, which would reduce the dataset to 299 rows from 920, alternatives like median and mode imputation were used. <br>
  - Used functions like `describe()`, `info()`, `value_counts()`, and examined unique values in each column. <br>
  - Explored relationships between features using various plots, including individual column plots and pairwise comparisons.
</h4>

<h2>2- Model :</h2>
<h4>
  - Built a prediction model with data preprocessing steps including encoding, scaling, and data splitting. <br>
  - Demonstrated the model's performance and saved the model, encoders (OneHot and Label Encoders), and the Standard Scaler. <br>
  - Provided an example on how to process input data to be compatible with the model, facilitating integration with the Flask app.
</h4>

<h2>3- App :</h2>
<h4>
  - Developed a Flask application to collect inputs from patients or doctors, process them, and use the model for predictions. <br>
  - Input processing in the app follows the same steps outlined in the model development phase.
</h4>

<h2>4- Templates:</h2>
<h4>
  - Includes `index.html`, a basic HTML page for input fields corresponding to model features, a predict button, and a section to display prediction results.
</h4>

<h3>Saved Files :</h3>
<h4>
  1. <strong>heart_disease_encoder.pkl</strong>: Saved Label Encoder. <br>
  2. <strong>heart_disease_model.keras</strong>: Saved prediction model. <br>
  3. <strong>heart_disease_OneHotEncoder.pkl</strong>: Saved OneHot Encoder. <br>
  4. <strong>heart_disease_standard_scaler.pkl</strong>: Saved Standard Scaler. <br>
  5. <strong>heart_disease_uci.csv</strong>: CSV file containing the dataset.
</h4>
