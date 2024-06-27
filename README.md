# Start-Up-Success-Prediction-Analysis-Using-Hybrid-Machine-Learning-Techniques-

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
This project aims to predict start-up success using hybrid machine learning algorithms. By integrating various models such as Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, Gradient Boosting, and Support Vector Machine, we achieve an accuracy of up to **96.22%**. The goal is to provide stakeholders with valuable insights for informed decision-making in the entrepreneurial ecosystem.

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
The dataset contains features related to start-up characteristics, including:
- Company details
- Team attributes
- Market presence
- Financial indicators
- Technological focus

**Note:** Due to class imbalance in the dataset, specific pre-processing steps such as handling missing values, label encoding, and feature selection using XGBoost are applied.

## Model Architecture
The proposed architecture encompasses the following steps:
1. **Data Acquisition and Pre-processing**
2. **Feature Selection using XGBoost**
3. **Hybrid Model Construction**
4. **Ensemble Model Development**
5. **Evaluation and Visualization**
6. **Deployment and Monitoring**

## Results
The hybrid model combining Gradient Boosting, Random Forest, and SVM achieved the highest accuracy of **96.22%**. The model performance is evaluated using various metrics including accuracy, precision, recall, and F1-score.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
