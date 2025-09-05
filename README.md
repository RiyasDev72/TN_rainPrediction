# TN_rainPrediction
Perfect! Thanks for sharing your actual project structure. Based on this, here’s a README tailored to your setup:

Tamil Nadu Rain Prediction

A machine learning project that predicts whether it will rain tomorrow in any district of Tamil Nadu, India. The project fetches weather data via an API, preprocesses it, trains a model using Logistic Regression, and allows predictions for user-specified districts.

Features

Fetches historical weather data for Tamil Nadu districts using an API.

Preprocesses data and saves it in a Parquet file for efficiency.

Trains a Logistic Regression model using scikit-learn.

Saves the trained model using Joblib for future predictions.

Predicts whether it will rain tomorrow based on user-input district name.

Installation

Clone this repository:

git clone https://github.com/USERNAME/REPO_NAME.git
cd REPO_NAME


Install dependencies (recommended in a virtual environment):

pip install -r requirements.txt


Dependencies include:

pandas

numpy

scikit-learn

joblib

requests (for API calls)

Usage

All the main work is done in the Jupyter Notebook:

Open the notebook:

jupyter notebook TN_rainPredicton.ipynb


The notebook contains all steps:

Fetch weather data for Tamil Nadu districts via API.

Preprocess and clean the data (TamilNaduWeather_AfterPreprocessing(NoDup,properindex).parquet).

Train a Logistic Regression model and save it (TN_rainPredicton_data.joblib).

Predict rain for a user-specified district.

To make predictions:

Run the prediction cells in the notebook.

Enter a district name when prompted.

Output: Rain tomorrow: Yes or Rain tomorrow: No.

Project Structure
├── tamil_nadu_rain_prediction_rows/           # Folder with raw or additional data
├── TamilNaduWeather_AfterPreprocessing(NoDup,properindex).parquet  # Preprocessed dataset
├── TN_rainPredicton.ipynb                     # Main Jupyter Notebook with full pipeline
├── TN_rainPredicton_data.joblib               # Trained Logistic Regression model
└── README.md                                  # This file

How it Works

Data Fetching: Collects weather data (temperature, humidity, wind, precipitation, etc.) for Tamil Nadu districts using an API.

Preprocessing: Cleans data, removes duplicates, ensures proper indexing, and saves it in Parquet format.

Model Training: Logistic Regression predicts RainTomorrow based on historical weather data.

Prediction: User enters a district name, and the trained model predicts whether it will rain tomorrow.


Made BY:
     GitHub username: RiyasDev72
     Email          : riyasdev72@gmail.com
