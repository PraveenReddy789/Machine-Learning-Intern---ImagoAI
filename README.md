# Machine-Learning-Intern---ImagoAI
# Hyperspectral Imaging for Mycotoxin Prediction

## Overview
This repository contains a machine learning pipeline for analyzing hyperspectral imaging data of corn samples. The model predicts DON (vomitoxin) concentration using dimensionality reduction techniques and an XGBoost regression model.

## Dataset
- **Features:** Spectral reflectance values across multiple wavelength bands.
- **Target Variable:** DON concentration (in ppb) for regression.
- **File:** `TASK-ML-INTERN.csv`

## Installation
Clone the repository and install dependencies:
```bash
git clone <repo_link>
cd <repo_name>
pip install -r requirements.txt
```

### Required Libraries
Ensure the following Python libraries are installed:
```bash
pip install numpy pandas matplotlib scikit-learn xgboost
```

## Running the Code
To train and evaluate the model, execute the Python script:
```bash
python src/hyperspectral_model.py
```

Alternatively, run the Jupyter Notebook if available:
```bash
jupyter notebook
```

## Model Workflow
1. **Data Preprocessing**
   - Handle missing values & normalize data.
   - Visualize spectral bands.
2. **Dimensionality Reduction**
   - Apply PCA (10 components) for feature reduction.
   - Visualize principal components.
3. **Model Training & Evaluation**
   - Train an XGBoost regression model.
   - Evaluate performance (MAE, RMSE, R² score).
   - Visualize actual vs. predicted values.

## Results
**Final Model Performance:**
- **MAE:** 1493.99
- **RMSE:** 2825.67
- **R² Score:** 0.97

## Contributors
- **Praveen Reddy Yallayyagari**

---
Feel free to open issues or contribute to this project!

