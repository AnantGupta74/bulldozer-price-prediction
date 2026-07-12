# 🚜 Bluebook for Bulldozers: Sale Price Prediction

## 📌 Project Overview
This project applies machine learning to predict the auction sale price of bulldozers based on their usage, equipment type, and configuration. Using the [Kaggle Bluebook for Bulldozers dataset](https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview), this notebook demonstrates a complete end-to-end data science workflow — from raw data to a tuned regression model.

## 🛠️ Technical Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib
- **Model:** RandomForestRegressor
- **Evaluation Metric:** RMSLE (Root Mean Squared Log Error)

## 🚀 Project Workflow
1. **Data Ingestion** — Loading time-series data with initial date parsing.
2. **Exploratory Data Analysis (EDA)** — Visualizing price distributions and identifying missing values.
3. **Feature Engineering** — Extracting temporal features (Year, Month, Day of week) from the `saledate` column.
4. **Preprocessing**
   - Converting string objects into Pandas Categories.
   - Handling missing numerical data via median imputation.
   - Binary encoding of missing status to preserve data context.
5. **Model Selection & Tuning**
   - Subset-based training for rapid experimentation.
   - Hyperparameter optimization using `RandomizedSearchCV`.
6. **Evaluation** — Validating model performance on time-segmented data.
7. **Feature Importance** — Analyzing key drivers behind bulldozer pricing.

## 📊 Key Results
- **Validation RMSLE:** ~0.245
- **R² Score:** ~0.88
- **Top Predictors:** Equipment age (`YearMade`), `ProductSize`, and `saleYear`.

## 📁 Repository Structure
```
bulldozer-price-prediction/
├── README.md
├── requirements.txt
├── notebooks/
│   └── bulldozer_price_prediction.ipynb
└── data/
    └── README.md   # instructions for downloading the dataset
```

## 📂 Dataset
This project uses the [Bluebook for Bulldozers dataset](https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview) from Kaggle. The raw data is **not included** in this repository due to Kaggle's competition data terms. To reproduce this project:

1. Download the dataset from the [Kaggle competition page](https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview) (requires a free Kaggle account and accepting the competition rules).
2. Place the CSV files in a local `data/` folder.
3. Update the file paths in the notebook if needed.

## ⚙️ How to Run
```bash
# Clone the repository
git clone https://github.com/<your-username>/bulldozer-price-prediction.git
cd bulldozer-price-prediction

# Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook notebooks/bulldozer_price_prediction.ipynb
```

## 📦 Dependencies
See [`requirements.txt`](./requirements.txt). Core libraries: Pandas, NumPy, Matplotlib, Scikit-Learn.

