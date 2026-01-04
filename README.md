# Customer Churn Prediction Project

## Project Overview
This project aims to build a machine learning model that predicts whether a customer will churn (leave the service) based on their demographic, account, and service-related data. The project includes comprehensive data exploration, preprocessing, model building, evaluation, and prediction capabilities.

## Project Structure
```
customer_churn_prediction/
├── 01_Data_Exploration_Preprocessing.ipynb  # Data loading, EDA, and preprocessing
├── 02_Model_Building.ipynb                  # Model training and hyperparameter tuning
├── 03_Model_Evaluation.ipynb                # Model evaluation and visualization
├── 04_Predict_New_Data.ipynb                # Prediction on new customer data
├── requirements.txt                          # Python dependencies
├── README.md                                 # Project documentation
├── data/                                     # Dataset directory
│   └── customer_data.csv                    # Input dataset (to be added)
└── models/                                   # Saved models directory
    ├── scaler.pkl
    ├── logistic_regression.pkl
    ├── random_forest.pkl
    └── (other model files)
```

## Installation

1. Clone or download this repository
2. Install required packages:
```bash
pip install -r requirements.txt
```

## Dataset

The dataset should be placed in the `data/` directory as `customer_data.csv`. 

**Dataset Source:** [Google Sheets Link](https://docs.google.com/spreadsheets/d/1rnBO9F9xdSUY-WpeOJilMxMRZT-hwwWq6O98OHreY0k/edit?gid=1602415961#gid=1602415961)

**To download the dataset:**
1. Open the Google Sheets link
2. Go to File → Download → Comma Separated Values (.csv)
3. Save as `customer_data.csv` in the `data/` folder

## Usage

### Step 1: Data Exploration and Preprocessing
Run `01_Data_Exploration_Preprocessing.ipynb` to:
- Load and explore the dataset
- Perform exploratory data analysis (EDA)
- Handle missing values and data inconsistencies
- Encode categorical variables
- Create new features
- Save processed data

### Step 2: Model Building
Run `02_Model_Building.ipynb` to:
- Split data into training and testing sets
- Scale features
- Train multiple models (Logistic Regression, Random Forest, XGBoost)
- Perform hyperparameter tuning
- Compare model performance
- Save trained models

### Step 3: Model Evaluation
Run `03_Model_Evaluation.ipynb` to:
- Evaluate model performance with multiple metrics
- Visualize confusion matrices
- Plot ROC curves and Precision-Recall curves
- Analyze feature importance
- Generate insights and recommendations

### Step 4: Predict New Data
Run `04_Predict_New_Data.ipynb` to:
- Load trained model
- Preprocess new customer data
- Make churn predictions
- Get prediction probabilities

## Features

The dataset contains the following features:
- **Demographic**: gender, SeniorCitizen, Partner, Dependents
- **Account**: tenure, Contract, PaperlessBilling, PaymentMethod
- **Services**: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
- **Charges**: MonthlyCharges, TotalCharges
- **Target**: Churn (Yes/No)

## Models Implemented

1. **Logistic Regression**: Baseline linear model
2. **Random Forest**: Ensemble tree-based model with hyperparameter tuning
3. **XGBoost**: Gradient boosting model (optional, requires xgboost package)

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- PR-AUC Score

## Expected Results

- Model accuracy: 75-85%
- ROC-AUC: 0.80-0.90
- Key insights on factors affecting churn

## Key Insights

Based on the analysis, common factors affecting churn include:
- Contract type (Month-to-month customers churn more)
- Tenure (Lower tenure = higher churn risk)
- Payment method (Electronic check has higher churn)
- Internet service type (Fiber optic customers churn more)
- Monthly charges (Higher charges = higher churn risk)

## Business Recommendations

1. **Target Month-to-month customers** for retention campaigns
2. **Offer incentives** to long-tenure customers
3. **Improve service quality** for fiber optic internet users
4. **Promote automatic payment methods** to reduce churn
5. **Create loyalty programs** for customers with high tenure

## Author
Student Project - Customer Churn Prediction

## License
This project is for educational purposes.

## Notes
- Make sure to run notebooks in sequence (01 → 02 → 03 → 04)
- Models are saved automatically after training
- Processed data is saved for reuse between notebooks

