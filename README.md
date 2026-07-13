# 🚜 Bulldozer Price Prediction

An end-to-end machine learning project that predicts the sale price of bulldozers using historical auction data from the Bluebook for Bulldozers Kaggle competition. This project demonstrates the complete machine learning workflow, including data exploration, preprocessing, feature engineering, model training, hyperparameter tuning, and evaluation.

---

## 📌 Project Overview

Accurately estimating the resale value of heavy equipment is important for buyers, sellers, and auction companies. In this project, a Random Forest Regressor is trained on historical auction data to predict bulldozer sale prices based on machine specifications, usage information, and sale dates.

This project was built as part of my machine learning learning journey to gain practical experience with regression problems and end-to-end ML pipelines.

---

## 🎯 Objectives

* Perform exploratory data analysis (EDA)
* Clean and preprocess real-world data
* Engineer useful features from datetime columns
* Train a machine learning regression model
* Tune model hyperparameters
* Evaluate model performance using RMSLE
* Understand feature importance

---

## 📂 Dataset

**Source:** Kaggle - Bluebook for Bulldozers Competition

The dataset is not included in this repository because of Kaggle's licensing policy.

Download the dataset from:

https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

After downloading, place the extracted files inside the `data/` folder.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## 📁 Project Structure

```text
bulldozer-price-prediction/
│
├── data/
│   ├── README.md
│   └── (Download Kaggle dataset here)
│
├── notebooks/
│   └── end_to_end_bulldozer_price_prediction.ipynb
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AnantGupta74/bulldozer-price-prediction.git
cd bulldozer-price-prediction
```

### 2. Create a virtual environment (optional but recommended)

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**macOS / Linux**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the dataset

Download the Bluebook for Bulldozers dataset from Kaggle and place all files inside the `data/` directory.

### 5. Run the notebook

```bash
jupyter notebook notebooks/end_to_end_bulldozer_price_prediction.ipynb
```

---

## 🔄 Machine Learning Workflow

1. Load and inspect the dataset
2. Explore missing values and data distribution
3. Perform feature engineering
4. Handle missing values
5. Convert categorical variables into numerical features
6. Train a Random Forest Regressor
7. Tune hyperparameters using RandomizedSearchCV
8. Evaluate the model using RMSLE
9. Analyze feature importance

---

## 📈 Model

**Algorithm Used**

* Random Forest Regressor

**Hyperparameter Tuning**

* RandomizedSearchCV

**Evaluation Metric**

* Root Mean Squared Log Error (RMSLE)

---

## 📊 Results

The tuned Random Forest model achieved an RMSLE of approximately **0.245** on the validation set.

---

## 📚 Key Concepts Practiced

* Regression
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Handling Missing Values
* Encoding Categorical Variables
* Random Forest Regression
* Hyperparameter Tuning
* Model Evaluation
* Feature Importance

---

## 🔮 Future Improvements

* Compare multiple regression models
* Build a reusable training pipeline
* Save and load trained models
* Create a simple prediction interface using Streamlit or Flask
* Experiment with gradient boosting models such as XGBoost or LightGBM

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgements

* Kaggle Bluebook for Bulldozers Competition
* Daniel Bourke & Andrei Neagoie Machine Learning Bootcamp
* Scikit-learn Documentation

---

## 👤 Author

**Anant Gupta**

GitHub: https://github.com/AnantGupta74
