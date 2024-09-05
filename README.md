<h1>Heart Disease Prediction Project</h1>

<h2>Project Overview</h2>
<p>This project aims to predict heart disease stages using a machine learning model deployed through a Flask web application. It involves data analysis, model development, and a user-friendly interface for inputting patient data and viewing predictions.</p>

<h2>Project Steps</h2>

<h3>1. Data Analysis</h3>
<ul>
  <li><strong>Objective:</strong> Analyze and clean the UCI Heart Disease dataset, handling missing values efficiently.</li>
  <li><strong>Missing Values:</strong> Instead of deleting rows (which would reduce the dataset from 920 to 299 rows), imputation with median and mode was used.</li>
  <li><strong>EDA (Exploratory Data Analysis):</strong>
    <ul>
      <li>Used functions like <code>describe()</code>, <code>info()</code>, and <code>value_counts()</code> to understand data distribution.</li>
      <li>Checked unique values in each column and explored feature relationships using plots.</li>
    </ul>
  </li>
</ul>

<h3>2. Model Development</h3>
<ul>
  <li><strong>Model Creation:</strong> Developed a predictive model with steps including encoding, scaling, and data splitting.</li>
  <li><strong>Performance and Saving:</strong> The model's performance was evaluated, and the following were saved:
    <ul>
      <li>Prediction model: <code>heart_disease_model.keras</code></li>
      <li>Encoders: <code>heart_disease_encoder.pkl</code> and <code>heart_disease_OneHotEncoder.pkl</code></li>
      <li>Standard Scaler: <code>heart_disease_standard_scaler.pkl</code></li>
    </ul>
  </li>
  <li><strong>Integration:</strong> Provided examples to ensure input data compatibility with the Flask app.</li>
</ul>

<h3>3. Flask Application</h3>
<ul>
  <li><strong>Purpose:</strong> Collect inputs from users, process them, and use the model for predictions.</li>
  <li><strong>Input Consistency:</strong> The app processes inputs using the same steps as the model development phase.</li>
</ul>

<h3>4. Templates</h3>
<ul>
  <li><code>index.html</code>: A basic HTML template with input fields matching model features, a prediction button, and a section to display results.</li>
</ul>

<h2>Saved Files</h2>
<ul>
  <li><code>heart_disease_encoder.pkl</code> - Saved Label Encoder.</li>
  <li><code>heart_disease_model.keras</code> - Saved Prediction Model.</li>
  <li><code>heart_disease_OneHotEncoder.pkl</code> - Saved OneHot Encoder.</li>
  <li><code>heart_disease_standard_scaler.pkl</code> - Saved Standard Scaler.</li>
  <li><code>heart_disease_uci.csv</code> - Dataset in CSV format.</li>
</ul>

<h2>Screenshots</h2>
<ul>
  <li><strong>Input Page (<code>0.png</code>):</strong> Displays how users enter feature values.</li>
  <li><strong>Prediction Result (<code>1(1).png</code>):</strong> Shows JSON output containing:
    <ul>
      <li><strong>Predicted Category:</strong> The category number with the highest probability.</li>
      <li><strong>Predicted Label:</strong> The meaning of the predicted category.</li>
      <li><strong>Prediction Probabilities:</strong> Probabilities for each class in the prediction.</li>
    </ul>
  </li>
</ul>

<h2>How to Run the Project</h2>

<h3>1. Set Up the Conda Environment</h3>
<p>Create and activate a conda environment with the required Python version:</p>
<pre><code>conda create --name heart_disease_env python=3.8</code></pre>
<pre><code>conda activate heart_disease_env</code></pre>

<h3>2. Install Required Libraries</h3>
<p>Create a <code>requirements.txt</code> file with the following content:</p>
<pre><code>
TensorFlow==2.13.0
Keras==2.13.1
Scikit-learn==1.3.2
Pandas==2.0.3
Matplotlib==3.7.5
Seaborn==0.13.2
Imbalanced-learn==0.12.3
Joblib==1.4.2
NumPy==1.24.3
Flask==3.0.3
</code></pre>
<p>Install the libraries using:</p>
<pre><code>pip install -r requirements.txt</code></pre>

<h3>3. Run the Application</h3>
<p>Run the Flask app using:</p>
<pre><code>python app.py</code></pre>
<p>Ensure that the directory contains:</p>
<ul>
  <li><strong>Model:</strong> <code>heart_disease_model.keras</code></li>
  <li><strong>Label Encoder:</strong> <code>heart_disease_encoder.pkl</code></li>
  <li><strong>OneHot Encoder:</strong> <code>heart_disease_OneHotEncoder.pkl</code></li>
  <li><strong>Standard Scaler:</strong> <code>heart_disease_standard_scaler.pkl</code></li>
</ul>
<p>Include a <code>templates</code> folder with the <code>index.html</code> file.</p>
