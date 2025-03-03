# definity
# Python Project
This is a simple Python project that uses machine learning to predict customer churn for a telecommunications company.
input dataset: telco custoemr churn
model: random forect classification
datapreprocessing: removed rows with missing vlaues. removed column customer id
feature encoding: converted categorical variables like gender, senior citizen to numerical variables for machine learning compatability
data splitting: Split the dataset into features (X) and target (y), where the target is the Churn column.
Split the data into training and testing sets with an 80-20% ratio using train_test_split from Scikit-Learn.
feature scaling: Scaled the features using StandardScaler to standardize them, which is important for many machine learning models like Random Forest.
 Model Training
Trained a Random Forest Classifier on the training data with 100 estimators (trees).
Predicted the Churn values for the test data.
Model Evaluation
Evaluated the model’s performance using accuracy, classification report, and a confusion matrix.

Results:
Overall Model Performance:
Accuracy: The model has an overall accuracy of 80%, which means it correctly predicted 80% of the total instances (both churn and non-churn).

Precision:

For Non-Churn (Class 0): 0.83 – High precision, indicating fewer false positives.
For Churn (Class 1): 0.66 – Lower precision, meaning there are more false positives for churned customers.

Recall:

For Non-Churn (Class 0): 0.91 – Very good recall, meaning the model captures most of the non-churned customers.
For Churn (Class 1): 0.49 – Poor recall, meaning the model is missing a lot of churned customers, which is a key problem.

F1-Score:

For Non-Churn (Class 0): 0.87 – Excellent balance of precision and recall.
For Churn (Class 1): 0.57 – The model's F1-score for churn is low, indicating an imbalance in performance between predicting churn vs. non-churn.
