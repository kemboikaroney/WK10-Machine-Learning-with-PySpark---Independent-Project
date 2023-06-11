# Telecom Customer Churn Prediction

This project aims to develop a machine learning model using PySpark to predict customer churn in a telecom company. By accurately identifying customers at risk of leaving, the company can implement proactive measures to retain them, reduce customer attrition, and improve overall business performance.

## Dataset

The telecom customer dataset used for this project is provided in the `telecom_dataset.csv` file. It includes relevant features such as customer demographics, usage patterns, service plans, call details, and churn status. The dataset has been preprocessed to handle missing values and encode categorical variables.

## Getting Started

To run the project, follow these steps:

1. Install the required dependencies by running `pip install -r requirements.txt`.
2. Ensure that you have Apache Spark installed and configured.
3. Place the `telecom_dataset.csv` file in the same directory as the Python script.
4. Run the `telecom_churn_prediction.py` script using Python.

## Implementation Details

The project is implemented in Python using the PySpark library. The main steps of the implementation are as follows:

1. Loading and Preprocessing: The dataset is loaded using SparkSession and preprocessed to handle missing values. Categorical variables are encoded using StringIndexer.

2. Feature Engineering: New features are created from the existing dataset, such as call duration, average monthly spend, customer tenure, or customer satisfaction scores. These features are calculated and added to the dataset.

3. Model Training: Two models, Random Forest Classifier and Logistic Regression, are selected for churn prediction. Hyperparameter tuning is performed using TrainValidationSplit to select the best model based on evaluation metrics.

4. Model Evaluation: The models are evaluated using the BinaryClassificationEvaluator, and the accuracy metric is calculated. The achieved accuracies for each model are reported.

## Results

The following results were obtained from the trained models:

- Random Forest Classifier Accuracy: 50%
- Logistic Regression Accuracy: 83.33%

The Logistic Regression model achieved the desired accuracy of 80% and outperformed the Random Forest Classifier.

## Documentation

For detailed documentation about the project, including dataset information, preprocessing steps, feature engineering, model selection, and evaluation results, refer to the pdf file [Telecom Customer Churn Prediction Documentation].

## Contributing

Contributions to this project are welcome. Feel free to open an issue or submit a pull request with any improvements or bug fixes.
