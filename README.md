Credit Card Fraud Detection


📋 Project Overview
This project aims to develop a classification model to detect fraudulent credit card transactions efficiently. The goal is to minimize false positives while maintaining high accuracy, ensuring robust fraud detection.

The dataset includes:

Transaction amount

Merchant details

Timestamps

Other anonymized features

We address class imbalance using oversampling, undersampling, and synthetic data generation techniques (SMOTE).

📚 Dataset
Dataset: Kaggle Credit Card Fraud Detection

Size: ~284,807 transactions

Positive Class (Fraudulent): ~0.172% of total transactions (highly imbalanced)

⚙️ Project Structure
bash
Copy
Edit
├── data/                # Dataset files
├── notebooks/           # Jupyter Notebooks for EDA, preprocessing, modeling
├── models/              # Trained models (if any)
├── src/                 # Python scripts for preprocessing, modeling
├── README.md            # Project overview and instructions
├── requirements.txt     # List of dependencies
└── LICENSE
🚀 Key Steps
1. Data Preprocessing
Handling Missing Values: Checked and confirmed no missing values.

Feature Scaling: Standardized transaction Amount and Time.

Feature Engineering:

Created transaction frequency per user.

Engineered location mismatch (based on merchant and transaction location).

Detected spending patterns anomalies.

2. Handling Imbalanced Data
Oversampling: Using SMOTE (Synthetic Minority Oversampling Technique).

Undersampling: Using NearMiss technique.

Compared results of oversampling vs undersampling strategies.

3. Model Building
Trained and compared multiple classification models:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Support Vector Machine (SVM)

K-Nearest Neighbors (KNN)

4. Model Evaluation
Used the following metrics:

Accuracy

Precision

Recall

F1-Score

ROC-AUC Score

Confusion Matrix

Emphasis was given to minimize False Positives while maintaining high Recall (detect more frauds).

🏆 Best Model

Metric	Value
Accuracy	99.93%
Precision	92.4%
Recall	84.5%
F1-Score	88.3%
ROC-AUC Score	98.9%
Best Performing Model: Random Forest Classifier (with SMOTE oversampling)

📈 Visualization Samples
Fraud vs Non-Fraud Class Distribution

t-SNE Plot for data visualization

Confusion Matrix

ROC-AUC Curve

📋 Requirements
Python 3.8+

pandas

numpy

scikit-learn

imbalanced-learn

matplotlib

seaborn

tensorflow (optional, for deep learning models)

🙌 Acknowledgements
Kaggle Credit Card Fraud Detection Dataset

📬 Contact
If you have any questions, feel free to reach out:

Sarthak Dey
