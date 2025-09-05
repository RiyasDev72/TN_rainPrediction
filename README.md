# TN_rainPrediction

A machine learning project that predicts whether it will rain tomorrow in any district of Tamil Nadu, India. The project fetches weather data via an **API**, preprocesses it, trains a model using **Logistic Regression**, and allows predictions for user-specified districts.

---

## ✨ Features

- Fetches historical weather data for Tamil Nadu districts using an **API**  
- Preprocesses data and saves it in a **Parquet file** for efficiency  
- Trains a **Logistic Regression model** using `scikit-learn`  
- Saves the trained model using **Joblib** for future predictions  
- Predicts whether it will rain tomorrow based on user-input **district name**  

---

## 🛠️ Installation

1. Clone this repository:

```bash
git clone https://github.com/RiyasDev72/TN_rainPrediction.git
cd TN_rainPrediction
```

2. Install the required dependencies:

```bash
pip install pandas numpy scikit-learn joblib requests
```

---

## 📊 Dependencies

- pandas
- numpy
- scikit-learn
- joblib
- requests (for API calls)

---

## 🚀 Usage

All the main work is done in the Jupyter Notebook:

1. Open the notebook:

```bash
jupyter notebook TN_rainPredicton.ipynb
```

2. The notebook contains all steps:
   - Fetch weather data via API
   - Preprocess and clean the data (`TamilNaduWeather_AfterPreprocessing(NoDup,properindex).parquet`)
   - Train a Logistic Regression model and save it (`TN_rainPredicton_data.joblib`)
   - Predict rain for a user-specified district

3. To make predictions:
   - Run the prediction cells in the notebook
   - Enter a district name when prompted
   - Output: `Rain tomorrow: Yes` or `Rain tomorrow: No`

---

## 📁 Project Structure

```
TN_rainPrediction/
├── tamil_nadu_rain_prediction_rows/                       # Folder with raw/additional data
├── TamilNaduWeather_AfterPreprocessing(NoDup,properindex).parquet  # Preprocessed dataset
├── TN_rainPredicton.ipynb                                 # Main Jupyter Notebook
├── TN_rainPredicton_data.joblib                           # Trained Logistic Regression model
└── README.md                                              
```

---

## 🔧 How it Works

1. **Data Fetching**: Collects weather data (temperature, humidity, wind, precipitation, etc.) for Tamil Nadu districts using an API
2. **Preprocessing**: Cleans data, removes duplicates, ensures proper indexing, and saves it in Parquet format
3. **Model Training**: Logistic Regression predicts RainTomorrow based on historical weather data
4. **Prediction**: User enters a district name, and the trained model predicts whether it will rain tomorrow

---

## 👨‍💻 Made By

**Riyas**  
- GitHub: [RiyasDev72](https://github.com/RiyasDev72)  
- Email: riyasdev72@gmail.com  

---
