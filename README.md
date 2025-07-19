💳 Credit Card Fraud Detection
This project uses machine learning to detect fraudulent credit card transactions. The dataset is highly imbalanced, and the model is designed to identify rare fraud cases with high precision and recall.

📌 Overview
Credit card fraud is a significant issue worldwide. Detecting fraudulent transactions early can help financial institutions and customers avoid severe losses. This project focuses on:

Building classification models to detect fraud

Handling class imbalance effectively

Evaluating models using appropriate metrics

📊 Dataset
Source: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud                                                                                   
Transactions: 284,807

Fraudulent: 492 (0.172%)

Features: 30 total, all numerical (PCA transformed), including:

Time, Amount, Class (target: 1 for fraud, 0 for normal)

🛠️ Technologies Used
Python

pandas, numpy

matplotlib, seaborn

scikit-learn

imbalanced-learn (for SMOTE)

🔍 Exploratory Data Analysis (EDA)
Analyzed class imbalance

Visualized distributions of Amount and Time

Correlation heatmaps and box plots for insights

⚙️ Preprocessing
Feature scaling using StandardScaler

Synthetic Minority Oversampling (SMOTE) to balance classes

Train-test split (typically 80/20)

🤖 Models Used
Logistic Regression

Decision Tree

Random Forest

XGBoost

Support Vector Machines (SVM)

📈 Evaluation Metrics
Due to class imbalance, we focus on:

Confusion Matrix

Precision, Recall, F1-score

ROC-AUC Score

PR AUC (Precision-Recall Curve)


📌 Key Results

Model                 	Precision	     Recall	      F1-score	       ROC-AUC

Logistic Regression	    ✅ High	      ✅ High	      ✅ High	       ✅ Good

XGBoost	                ✅ Higher	    ✅ Higher	    ✅ Better	       ✅ Best

XGBoost delivered the best results on fraud detection with balanced metrics.
