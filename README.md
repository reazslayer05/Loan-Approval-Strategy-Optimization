## Loan Approval Strategy Optimization

This project aims to optimize the loan approval strategy using machine learning techniques. The goal is to predict whether a loan application will be approved or denied based on various applicant features and financial data. The dataset includes information about applicants, and the objective is to predict if the loan should be approved ("Y") or denied ("N").

### Deployed Application

An application has been deployed to allow users to check the status of their loan approval. The app uses the trained machine learning models to predict loan approval based on the provided applicant details.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Modeling Process](#modeling-process)
4. [Results](#results)
5. [Installation and Setup](#installation-and-setup)
6. [Usage](#usage)
7. [Conclusion](#conclusion)
8. [License](#license)

## Project Overview

In this project, we aim to develop a machine learning model that helps in making informed loan approval decisions. The project explores various classification models, such as Logistic Regression, Decision Tree, and Random Forest, to determine the best approach for predicting loan approval outcomes.

## Data Description

The dataset includes the following features:

- **Applicant Demographics:** Information such as age, gender, marital status, education, etc.
- **Loan Details:** Loan amount, loan term, purpose, etc.
- **Financial Information:** Applicant’s income, credit score, existing debts, and financial history.
- **Target Variable:**
  - `Y`: The loan was approved.
  - `N`: The loan was denied.

### Example of Data Columns:
| Feature              | Description                             |
|----------------------|-----------------------------------------|
| Age                  | Age of the applicant                    |
| Credit Score         | Credit score of the applicant           |
| Loan Amount          | Amount requested by the applicant       |
| Annual Income        | Annual income of the applicant          |
| Loan Approval (Target) | Whether the loan was approved (Y) or denied (N) |

## Modeling Process

### 1. Data Preprocessing
The dataset was cleaned and preprocessed, including:
- Handling missing values
- Encoding categorical features
- Scaling numerical features to improve model performance

### 2. Model Training
The following machine learning models were used for training:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**

### 3. Model Evaluation
The models were evaluated based on accuracy, precision, recall, F1-score, and confusion matrix to select the best model for loan approval prediction.

## Results

| Model               | Accuracy  | Precision (Y) | Recall (Y) | F1-Score (Y) |
|---------------------|-----------|---------------|------------|--------------|
| Logistic Regression  | 0.79      | 0.76          | 0.99       | 0.86         |
| Decision Tree        | 0.69      | 0.76          | 0.78       | 0.77         |
| Random Forest        | 0.76      | 0.75          | 0.94       | 0.83         |

**Logistic Regression** outperformed other models with high recall for the positive class (Y), meaning it is very good at identifying loan approval cases.

## Installation and Setup

To run this project, ensure you have Python 3.x installed. It's recommended to use a virtual environment to keep dependencies isolated.

1. Clone the repository:

   git clone https://github.com/your-username/loan-approval-strategy-optimization

2. Install required dependencies:

   pip install -r requirements.txt

3. Run the project:
To run the Jupyter notebook for exploration and model development:

  jupyter notebook

## Usage

The project is implemented in a Jupyter notebook, where the following tasks are performed:

**Data Preprocessing**: Cleaning, encoding, and scaling the data.

**Model Training**: Training Logistic Regression, Decision Tree, and Random Forest models.

**Model Evaluation**: Evaluating the models using key performance metrics.

You can use the provided code to experiment with other models or datasets to improve the loan approval prediction system.

## Conclusion

**Logistic Regression** emerged as the best model with a high recall rate, indicating its effectiveness in detecting loan approval cases.

The project demonstrates how machine learning can be used to optimize loan approval strategies, aiding financial institutions in making more accurate and data-driven decisions.

An application has been deployed to check the status of loan approval, enabling users to interact with the model in a user-friendly way.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
