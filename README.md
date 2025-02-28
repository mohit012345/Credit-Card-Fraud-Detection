# Credit-Card-Fraud-Detection

Overview

This project implements a Random Forest Classifier to detect fraudulent credit card transactions. The model is trained using Python, scikit-learn, and pandas on a dataset containing transaction details.

 Dataset

The dataset used is from Kaggle's Credit Card Fraud Detection dataset, containing anonymized transaction features.

Features:
Time: Seconds elapsed between transactions
V1 to V28: Anonymized numerical features
Amount: Transaction amount
Class: 0 = Legitimate, 1 = Fraudulent (Target Variable)

 Dependencies

Ensure you have the required Python libraries installed:
pip install pandas numpy matplotlib seaborn scikit-learn

 Project Structure

Credit-Card-Fraud-Detection/
│-- creditcard.csv          
│-- fraud_detection.py      
│-- README.md               

Model Training & Evaluation

The dataset is processed as follows:
Data Preprocessing: Feature scaling using StandardScaler
Train-Test Split: 80% training, 20% testing
Random Forest Model: Trained with 20 trees for efficiency

Evaluation Metrics:

Accuracy Score
Precision & Recall
Confusion Matrix
ROC-AUC Score

Results Visualization

A confusion matrix is plotted to visualize model performance:
plt.figure(figsize=(6,4))
sns.heatmap(confusion_matrix(y_test, y_pred), annot=True, fmt='d', cmap='Blues')
plt.xlabel("Predicted")
plt.ylabel("Actual")
plt.title("Confusion Matrix")
plt.show()

 How to Run the Project

1)Clone this repository:
git clone https://github.com/YOUR_USERNAME/Credit-Card-Fraud-Detection.git

2)Navigate to the project folder:
cd Credit-Card-Fraud-Detection

3)Run the Python script:
python fraud_detection.py

Contributing
Feel free to fork this repository and suggest improvements!

 License
This project is open-source and available under the MIT License.

