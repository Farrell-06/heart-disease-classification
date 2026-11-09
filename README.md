# Heart Disease Classification Using Machine Learning

Machine learning model implementation to predict the risk of heart disease in patients based on clinical diagnostic parameters using the Support Vector Machine (SVM) algorithm.

## Overview

This project focuses on building, evaluating, and analyzing a supervised binary classification model for heart disease risk detection. By utilizing the Cleveland Heart Disease dataset, the workflow covers data cleaning, exploratory data analysis (EDA), correlation analysis, feature scaling, model training with Radial Basis Function (RBF) kernel, and comprehensive metric evaluation.

## Project Objectives

- Conduct thorough exploratory data analysis on clinical cardiovascular parameters.
- Handle preprocessing, duplicate data detection, and numerical feature standardization using \StandardScaler\.
- Train a Support Vector Machine (\SVC\) classification model optimized for non-linear decision boundaries.
- Evaluate model efficacy with confusion matrix, accuracy, precision, recall, and F1-score metrics, with high sensitivity (recall) on positive heart disease cases.

## Key Features

- **Exploratory Data Analysis (EDA):** Statistical summaries, correlation heatmaps, feature distribution plots, and target attribute breakdown.
- **Data Preprocessing Pipeline:** Handling feature scaling to normalize multi-scale clinical variables.
- **SVM Model with RBF Kernel:** Hyperparameters configured (\kernel='rbf'\, \C=1\, \gamma='scale'\, \probability=True\, \andom_state=42\).
- **Comprehensive Evaluation:** Confusion matrix visualization and detailed classification reporting.

## Technology Stack

- **Language:** Python
- **Environment:** Jupyter Notebook
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn

## Dataset Description

- **Source:** Cleveland Heart Disease Dataset
- **Total Records:** 303 patient records
- **Total Features:** 14 diagnostic attributes
  - \ge\: Age in years
  - \sex\: Biological sex (1 = male, 0 = female)
  - \cp\: Chest pain type (4 values: typical angina, atypical angina, non-anginal pain, asymptomatic)
  - \	restbps\: Resting blood pressure (in mm Hg on admission)
  - \chol\: Serum cholesterol in mg/dl
  - \bs\: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
  - \estecg\: Resting electrocardiographic results
  - \	halach\: Maximum heart rate achieved
  - \exang\: Exercise induced angina (1 = yes, 0 = no)
  - \oldpeak\: ST depression induced by exercise relative to rest
  - \slope\: The slope of the peak exercise ST segment
  - \ca\: Number of major vessels (0-3) colored by flourosopy
  - \	hal\: Thalassemia status (3 = normal, 6 = fixed defect, 7 = reversable defect)
  - \	arget\: Diagnosis of heart disease (1 = disease present, 0 = disease absent)

## Verified Performance Metrics

The model achieves the following evaluated performance on test data:

- **Training Accuracy:** 90.87%
- **Testing Accuracy:** 83.61%
- **Recall (Positive Class 1 - Disease Detection):** 94.00%
- **Precision (Class 0):** 91.00%
- **F1-Score (Positive Class 1):** 86.00%

> High recall on the positive class ensures minimal false negatives, an essential priority when screening potential medical conditions.

## Project Structure

\\\
heart-disease-classification/
├── heart-disease.csv       # Cleveland Heart Disease dataset
├── heart-disease.ipynb     # Jupyter Notebook containing analysis & model
├── requirements.txt        # Python dependency specifications
├── .gitignore              # Git ignore rules
└── README.md               # Project documentation
\\\

## Installation and Execution

1. **Clone this repository:**
   \\\ash
   git clone https://github.com/Farrell-06/heart-disease-classification.git
   cd heart-disease-classification
   \\\

2. **Create and activate a virtual environment (optional but recommended):**
   \\\ash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   \\\

3. **Install dependencies:**
   \\\ash
   pip install -r requirements.txt
   \\\

4. **Launch Jupyter Notebook:**
   \\\ash
   jupyter notebook heart-disease.ipynb
   \\\

## Academic Disclaimer

This project is an academic machine learning study developed for educational and portfolio demonstration purposes. The trained model is not an approved medical diagnostic instrument and must not be used as clinical diagnostic advice.

## Author

- **Farrell Putra Prayoga**
  - Portfolio: [farrellputra.site](https://farrellputra.site)
  - GitHub: [@Farrell-06](https://github.com/Farrell-06)
  - Program: Information Systems (S1 Sistem Informasi), Universitas Mercu Buana
