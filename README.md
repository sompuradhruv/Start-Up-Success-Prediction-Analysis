# Start-Up Success Prediction Analysis Using Hybrid Machine Learning Techniques

## Table of Contents
- [**Project Overview**](#project-overview)
- [**Installation**](#installation)
- [**Dataset**](#dataset)
- [**Model Architecture**](#model-architecture)
- [**Results**](#results)

## Project Overview
This project focuses on predicting the success of start-ups using a hybrid machine learning approach. Start-ups are known for their high-risk environment, where failure rates can be significant due to various factors such as market volatility, resource limitations, and execution challenges. Our goal is to leverage machine learning techniques, specifically combining Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, Gradient Boosting, and Support Vector Machine models, to provide stakeholders with reliable predictions. By achieving an accuracy of up to **96.22%**, our model aims to assist investors, incubators, and entrepreneurs in making informed decisions and mitigating risks in the start-up ecosystem.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/sompuradhruv/startup-success-prediction-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd startup-success-prediction-analysis
    ```
3. Create and activate a virtual environment:
    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```
4. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Dataset
The dataset used in this project includes a comprehensive set of features that capture various aspects of start-up ventures:
- **Company details**: Incorporation date, location, industry sector.
- **Team attributes**: Founder background, team size, experience.
- **Market presence**: Customer segments, market share, competitive landscape.
- **Financial indicators**: Funding rounds, revenue, profitability.
- **Technological focus**: Product/service innovation, technology stack.

Given the nature of start-up data, our dataset exhibits class imbalance, with successful start-ups comprising 64.6% and unsuccessful ones 35.4%. To address this, we apply robust preprocessing techniques, including handling missing values, label encoding categorical variables, and feature selection using XGBoost to prioritize influential features.

### Dataset Heatmap

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/f39d28fb-e450-4c4b-b47d-e61e133912d3)

### Pie Chat distribution of target variable

![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/026dc0a3-cacd-4471-b537-81611bc08d03)

### Corelation Matrix of the dataset

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/cb89396d-c38a-470a-b170-c373de397152)


## Model Architecture
The project follows a structured approach:

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/6bcb5848-da11-4ced-9b2b-ce2888f71d74)

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/6fb29a13-8e07-4d84-afb6-8f01d3a2f551)


1. **Data Acquisition and Pre-processing**: Cleaning data, handling missing values, and preparing features for analysis.
2. **Feature Selection using XGBoost**: Identifying key features significantly impacting start-up success.

      ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/1514854b-b845-4340-ada7-8c3e045f1447)

4. **Hybrid Model Construction**: Integrating multiple machine learning algorithms to create a robust predictive model.
5. **Ensemble Model Development**: Building an ensemble model using VotingClassifier to leverage the strengths of individual algorithms.

      ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/89329861-538f-4065-b1ff-bb83dfd57645)

7. **Evaluation and Visualization**: Assessing model performance using metrics such as accuracy, precision, recall, and F1-score. Visualizing results to gain insights into model behavior.

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/e6911c4d-e191-444d-8164-0da75285e7ca)

### Confusion Matrix

   ![image](https://github.com/sompuradhruv/Start-Up-Success-Prediction-Analysis/assets/78086198/37e0c923-1207-466a-9a85-df3ae02e82dd)


## Results
The hybrid model combining Gradient Boosting, Random Forest, and SVM achieved the following results:

| **Hybrid Algorithms**                            | **Accuracy** | **F1-Score** | **Precision** | **Recall** |
|--------------------------------------------------|--------------|--------------|---------------|------------|
| Logistic Regression and K-Nearest Neighbors      | 93.53%       | 94.77%       | 94.57%        | 94.63%     |
| Random Forest and Naïve Bayes                    | 94.58%       | 94.67%       | 94.57%        | 94.43%     |
| Ensemble of Gradient Boosting, Random Forest, and SVM | 96.22%       | 97.34%       | 97.22%        | 97.43%     |

These results demonstrate the efficacy of our approach in predicting start-up success with high accuracy and reliability.

