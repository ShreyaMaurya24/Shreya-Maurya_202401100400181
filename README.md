Loan Default Prediction using Random Forest

Overview

aThis project demonstrates how to predict whether a borrower will default on a loan using financial and credit-related data. A Random Forest Classifier is applied for classification, and the model's performance is evaluated using accuracy, precision, recall, and a confusion matrix heatmap.

How to Use

Run the notebook in Google Colab.

Upload your dataset in CSV format when prompted (e.g., Predict_Loan_Default.csv).

The model will preprocess the data, train using Random Forest, and output evaluation metrics.

Requirements

Python 3

Google Colab or Jupyter Notebook

Python Libraries Used

pandas
numpy
seaborn
matplotlib
scikit-learn
google.colab (for file upload)

Dataset Format

Your dataset should include:

Features relevant to a borrower's financial and credit history

A binary target column named Default (1 = Default, 0 = No Default)

Optional: A LoanID column which will be dropped during preprocessing

Example columns:

['LoanID', 'Credit_Score', 'Income', 'Employment_Status', 'Loan_Amount', 'Default']

Steps in the Code

File Upload: File is uploaded using Google Colab's files.upload().

Data Loading: CSV is read using pandas.

Preprocessing:

Drop irrelevant columns like LoanID

Handle missing values (rows with missing data are dropped)

Encode categorical variables using LabelEncoder

Scale features using StandardScaler

Model Training: A RandomForestClassifier is trained on 80% of the data.

Prediction and Evaluation:

Predictions made on test set

Confusion matrix is visualized with Seaborn

Evaluation metrics printed: Accuracy, Precision, Recall, F1 Score, Classification Report

Output Example

✅ Accuracy: 0.92
✅ Precision: 0.89
✅ Recall: 0.85

A confusion matrix heatmap will be shown below these metrics.

Notes

Make sure your dataset has a column named Default.

Categorical variables are encoded using LabelEncoder.

Feature scaling is applied before training.

License

This project is open-source and can be used for learning and academic purposes.# Shreya-Maurya_202401100400181
