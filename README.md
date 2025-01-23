
# Online Payment Fraud Detection

This repository contains a machine learning project aimed at detecting fraudulent transactions in online payment systems. By analyzing transaction data, the system identifies patterns and anomalies that could indicate fraudulent activity. 

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Features](#features)
- [Project Workflow](#project-workflow)
- [Modeling](#modeling)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Fraud detection is a critical component of online payment systems. With the increasing volume of transactions, automating the detection process is essential to prevent losses. This project employs machine learning techniques to classify transactions as fraudulent or legitimate, helping reduce the risk of fraud in financial systems.

## Dataset
The dataset used for this project contains records of online transactions. Each transaction includes features like transaction type, amount, origin account, destination account, and labels indicating whether the transaction is fraudulent (`isFraud`).

## Key Features
- **step**: Time step of the transaction.
- **type**: Type of transaction (e.g., PAYMENT, TRANSFER, CASH_OUT).
- **amount**: Transaction amount.
- **nameOrig**: ID of the originating account.
- **oldbalanceOrg**: Balance of the originating account before the transaction.
- **newbalanceOrig**: Balance of the originating account after the transaction.
- **nameDest**: ID of the destination account.
- **oldbalanceDest**: Balance of the destination account before the transaction.
- **newbalanceDest**: Balance of the destination account after the transaction.
- **isFraud**: Label indicating if the transaction is fraudulent.
- **isFlaggedFraud**: Transactions flagged as suspicious by the system.

## Project Workflow
1. **Data Preprocessing**:
   - Handle missing or invalid values.
   - Encode categorical features.
   - Normalize numerical features for better model performance.

2. **Exploratory Data Analysis (EDA)**:
   - Analyze distributions, correlations, and trends in the dataset.
   - Identify key features that influence fraud detection.

3. **Feature Engineering**:
   - Transform features for better model interpretability and performance.

4. **Modeling**:
   - Train various machine learning models, including:
     - Logistic Regression
     - Decision Trees
     - Random Forests
     - Gradient Boosting
   - Evaluate models using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

5. **Prediction and Deployment**:
   - Use the trained model to classify new transactions as fraudulent or legitimate.

## Results
The project demonstrates the ability to detect fraudulent transactions with high precision and recall, minimizing false positives and negatives. Detailed evaluation metrics for the models are provided in the project files.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/srijanid/Online-Payment-Fraud-Detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Online-Payment-Fraud-Detection
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Preprocess the data:
   - Run the preprocessing script to clean and transform the dataset.

2. Train the model:
   - Use the provided scripts to train the machine learning models.

3. Evaluate the model:
   - Evaluate the model's performance using test data.

4. Make predictions:
   - Use the trained model to classify new transactions.

Example command to run the project:
```bash
python fraud_detection.py
```

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

---
