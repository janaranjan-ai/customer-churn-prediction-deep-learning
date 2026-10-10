# Customer Churn Prediction Using Deep Learning

A machine learning project that explores customer churn patterns and predicts whether a telecom customer is likely to leave the service using Exploratory Data Analysis (EDA) and an Artificial Neural Network (ANN).

## Project Overview

Customer churn is a major challenge for telecommunications companies. Understanding why customers leave helps businesses improve customer satisfaction and retention.

This project analyzes customer information, visualizes churn patterns, preprocesses the dataset, and builds a deep learning model to predict customer churn.

## Objectives

- Perform Exploratory Data Analysis (EDA).
- Visualize customer churn patterns and relationships between features.
- Clean and preprocess the dataset.
- Build an Artificial Neural Network using TensorFlow and Keras.
- Evaluate the model using classification metrics and visualizations.

## Dataset

**Dataset:** Telco Customer Churn

**Source:** IBM Sample Data Sets

The dataset contains approximately 7,043 customer records and 21 columns, including:

- Customer demographics
- Tenure
- Contract type
- Monthly charges
- Total charges
- Internet and phone services
- Churn status

The target variable is `Churn`, which indicates whether a customer left the service.

## Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow and Keras

## Exploratory Data Analysis

The project includes visualizations for:

1. Customer churn distribution
2. Customer churn by contract type
3. Customer tenure distribution by churn status
4. Monthly charges by churn status
5. Correlation heatmap of numerical features

## Model Architecture

The project uses an Artificial Neural Network (ANN) with:

- Dense layer with 64 neurons and ReLU activation
- Dropout layer with a rate of 0.2
- Dense layer with 32 neurons and ReLU activation
- Dropout layer with a rate of 0.2
- Output layer with one neuron and sigmoid activation

The model is compiled using the Adam optimizer and binary cross-entropy loss. Early stopping is used to help reduce overfitting.

## Model Evaluation

The model is evaluated using accuracy, precision, recall, F1-score, ROC-AUC, a confusion matrix, and an ROC curve.

**Recorded evaluation results:**

| Metric | Score |
|---|---:|
| Accuracy | 79.06% |
| Precision | 62.23% |
| Recall | 53.74% |
| F1-score | 57.68% |
| ROC-AUC | 0.8386 |

These results are from the current model run and may vary if the model is retrained with different settings.

## Project Structure

```text
customer-churn-prediction-deep-learning/
├── Customer_Churn_Prediction.ipynb
├── Customer_Churn_Prediction_Report.docx
├── customer_churn_actual_graphs.zip
├── README.md
└── WA_Fn-UseC_-Telco-Customer-Churn.csv
```

*Update the filenames in this structure to match the files you actually upload.*

## How to Run

1. Clone or download this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Upload the Telco Customer Churn dataset.
4. Install any missing dependencies.
5. Run the notebook cells in order.
6. Review the EDA visualizations and model evaluation results.

## Key Findings

- Month-to-month contracts account for a large number of churn cases.
- Churn is more concentrated among customers with shorter tenure.
- Customers who churned had a higher median monthly charge in the analyzed dataset.
- The model achieved an ROC-AUC of approximately 0.84 in the recorded evaluation.

These findings describe patterns in the dataset and do not necessarily establish causation.

## Future Improvements

- Compare the ANN with Logistic Regression, Random Forest, and Gradient Boosting.
- Tune model hyperparameters.
- Improve recall for customers likely to churn.
- Add explainability techniques to understand important churn factors.
- Build a simple web application for interactive predictions.

## Author

**Janaranjan K**  
B.Tech – Artificial Intelligence and Data Science  
KPR Institute of Engineering and Technology, Coimbatore

## Disclaimer

This project is intended for educational and academic purposes. Model predictions are not guaranteed to represent real-world customer behavior.
