# Start-Up Success Prediction Analysis Using Hybrid Machine Learning Techniques

## Table of Contents
- [**Project Overview**](#project-overview)
- [**Installation**](#installation)
- [**Usage**](#usage)
- [**Dataset**](#dataset)
- [**Model Architecture**](#model-architecture)
- [**Results**](#results)
- [**Contributing**](#contributing)
- [**License**](#license)

## Project Overview
This project focuses on predicting the success of start-ups using a hybrid machine learning approach. Start-ups are known for their high-risk environment, where failure rates can be significant due to various factors such as market volatility, resource limitations, and execution challenges. Our goal is to leverage machine learning techniques, specifically combining Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, Gradient Boosting, and Support Vector Machine models, to provide stakeholders with reliable predictions. By achieving an accuracy of up to **96.22%**, our model aims to assist investors, incubators, and entrepreneurs in making informed decisions and mitigating risks in the start-up ecosystem.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/startup-success-prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd startup-success-prediction
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

## Usage
1. Preprocess the data:
    ```bash
    python preprocess_data.py
    ```
2. Train the model:
    ```bash
    python train_model.py
    ```
3. Evaluate the model:
    ```bash
    python evaluate_model.py
    ```

## Dataset
The dataset used in this project includes a comprehensive set of features that capture various aspects of start-up ventures:
- **Company details**: Incorporation date, location, industry sector.
- **Team attributes**: Founder background, team size, experience.
- **Market presence**: Customer segments, market share, competitive landscape.
- **Financial indicators**: Funding rounds, revenue, profitability.
- **Technological focus**: Product/service innovation, technology stack.

Given the nature of start-up data, our dataset exhibits class imbalance, with successful start-ups comprising 64.6% and unsuccessful ones 35.4%. To address this, we apply robust preprocessing techniques, including handling missing values, label encoding categorical variables, and feature selection using XGBoost to prioritize influential features.

## Model Architecture
The project follows a structured approach:
1. **Data Acquisition and Pre-processing**: Cleaning data, handling missing values, and preparing features for analysis.
2. **Feature Selection using XGBoost**: Identifying key features that significantly impact start-up success.
3. **Hybrid Model Construction**: Integrating multiple machine learning algorithms to create a robust predictive model.
4. **Ensemble Model Development**: Building an ensemble model using VotingClassifier to leverage the strengths of individual algorithms.
5. **Evaluation and Visualization**: Assessing model performance using metrics such as accuracy, precision, recall, and F1-score. Visualizing results to gain insights into model behavior.

## Results
The hybrid model combining Gradient Boosting, Random Forest, and SVM achieved the following results:

| **Hybrid Algorithms**                            | **Accuracy** | **F1-Score** | **Precision** | **Recall** |
|--------------------------------------------------|--------------|--------------|---------------|------------|
| Logistic Regression and K-Nearest Neighbors      | 93.53%       | 94.77%       | 94.57%        | 94.63%     |
| Random Forest and Naïve Bayes                    | 94.58%       | 94.67%       | 94.57%        | 94.43%     |
| Ensemble of Gradient Boosting, Random Forest, and SVM | 96.22%       | 97.34%       | 97.22%        | 97.43%     |

These results demonstrate the efficacy of our approach in predicting start-up success with high accuracy and reliability.

## Contributing
Contributions to this project are welcome! If you have suggestions for improvements, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
