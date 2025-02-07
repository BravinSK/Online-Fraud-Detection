# Online Fraud Detection System

## Overview
The Online Fraud Detection System is a machine learning-based application that analyzes financial transactions to detect fraudulent activities. This project uses **Logistic Regression** and **Random Forest Classifier** to classify transactions as legitimate or fraudulent. The system also incorporates data preprocessing techniques and handles imbalanced datasets using **SMOTE (Synthetic Minority Over-sampling Technique)** and **Random Undersampling**.

## Features
- **Supervised Learning Models:** Utilizes **Logistic Regression** and **Random Forest Classifier** for fraud detection.
- **Imbalanced Data Handling:** Uses **SMOTE** and **Random Undersampling** to improve model performance.
- **Feature Engineering:** Prepares and optimizes datasets for enhanced model accuracy.
- **Hyperparameter Tuning:** Implements **Grid Search** to optimize model parameters.
- **Evaluation Metrics:** Uses **confusion matrix, accuracy score, and ROC-AUC curves** for model assessment.

## Technologies Used
- **Python**
- **scikit-learn**
- **pandas**
- **matplotlib & seaborn** (for visualization)
- **imbalanced-learn** (for data balancing)
- **Google Colab** (for model training)

## Dataset
The dataset contains transaction records with the following attributes:
- `step`: Represents the time step of the transaction.
- `type`: Type of transaction (TRANSFER, CASH_OUT, etc.).
- `amount`: Transaction amount.
- `nameOrig` & `nameDest`: Sender and receiver identifiers.
- `oldbalanceOrg` & `newbalanceOrig`: Sender's account balances before and after the transaction.
- `oldbalanceDest` & `newbalanceDest`: Receiver's account balances before and after the transaction.
- `isFraud`: Target variable indicating whether the transaction is fraudulent.
- `isFlaggedFraud`: Indicates flagged transactions by the system.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/YourUsername/Online-Fraud-Detection.git
   ```
2. Navigate to the project folder:
   ```sh
   cd Online-Fraud-Detection
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
1. Load the dataset into Google Colab or Jupyter Notebook.
2. Run the preprocessing steps to clean and prepare the data.
3. Train the machine learning models using the provided scripts.
4. Evaluate the models and visualize results using confusion matrices and ROC curves.

## Model Performance
| Model               | Accuracy | AUC Score |
|---------------------|---------|-----------|
| Logistic Regression | 93.26%  | 0.91      |
| Random Forest      | 99.92%  | 0.99      |

## Results
- The **Random Forest Classifier** outperformed Logistic Regression with **99.92% accuracy**.
- The **SMOTE technique** significantly improved the performance on imbalanced data.
- The fraud detection system provides an effective way to analyze transaction data and detect fraudulent activities in real-time.



