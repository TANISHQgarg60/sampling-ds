Credit Card Fraud Detection with SMOTE and Machine Learning

This project focuses on detecting credit card fraud using machine learning techniques and addressing data imbalance with SMOTE (Synthetic Minority Oversampling Technique). The dataset is highly imbalanced, so different sampling methods are applied to ensure fair evaluation of multiple classification models.

Features

Data Preprocessing:

Data loading and inspection.

Addressing class imbalance using SMOTE.

Sampling Techniques:

Systematic and random sampling techniques to create multiple datasets.

Model Evaluation:

Five machine learning models evaluated:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Support Vector Classifier

K-Nearest Neighbors Classifier

Accuracy Analysis:

Results presented as an accuracy matrix for all sampling techniques and models.

Best sampling technique identified for each model.

Dataset

The dataset used is Creditcard_data.csv, which contains the following:

Features:

V1 to V28: Principal components from PCA (anonymized for privacy).

Time: Transaction timestamp.

Amount: Transaction amount.

Target:

Class: Binary label (0 for non-fraud, 1 for fraud).

Workflow

1. Install Dependencies

Install the required Python libraries:

pip install pandas scikit-learn imbalanced-learn numpy

2. Data Preprocessing

Load the dataset and inspect its structure.

Apply SMOTE to handle the class imbalance (original distribution: 763 non-fraud and 9 fraud cases).

3. Sampling Techniques

Five datasets are created using different sampling techniques (random and systematic sampling).

4. Model Training and Evaluation

Split each sampled dataset into training (70%) and testing (30%).

Train and evaluate the following models:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Support Vector Classifier

K-Nearest Neighbors Classifier

5. Results

Generate an accuracy matrix summarizing the performance of each model for all sampling strategies.

Identify the best sampling technique for each model.

Save results to a CSV file (result.csv).

Results

Sample accuracy matrix:

Sampling Technique

Logistic Regression

Decision Tree

Random Forest

SVC

KNN

Sampling1

91.33%

98.67%

99.67%

70.67%

86.33%

Sampling2

91.67%

96.67%

98.67%

67.33%

79.67%

Sampling3

90.61%

98.25%

99.34%

67.69%

84.72%

Sampling4

94.33%

96.33%

99.67%

65.67%

83.00%

Sampling5

92.67%

98.00%

100.00%

67.33%

80.67%

Best sampling techniques for each model:

Logistic Regression: Sampling4

Decision Tree: Sampling1

Random Forest: Sampling5

Support Vector Classifier: Sampling1

K-Nearest Neighbors: Sampling1

Files

Creditcard_data.csv: Dataset used in this project.

result.csv: Accuracy matrix for all models and sampling techniques.

fraud_detection.py: Python script containing the full implementation.

Usage

Clone the repository:

git clone https://github.com/yourusername/credit-card-fraud-detection.git

Navigate to the directory:

cd credit-card-fraud-detection

Run the Python script:

python fraud_detection.py

Requirements

Python 3.7+

pandas

scikit-learn

imbalanced-learn

numpy

Acknowledgments

This project is inspired by the challenge of detecting fraud in real-world financial datasets and highlights the importance of handling data imbalance in machine learning workflows.

License

This project is licensed under the MIT License. See the LICENSE file for details.


