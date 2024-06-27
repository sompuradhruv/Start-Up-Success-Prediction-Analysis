# Start-Up Success Prediction Analysis Using Hybrid Machine Learning Techniques

## Authors

- Dhruv Umesh Sompura
- Priyadarshan Jain
- Dr. Malaserene

*School of Computer Science Engineering and Information Systems, Vellore Institute of Technology, Vellore, 632014, Tamil Nadu, India*

*Corresponding author’s Email: imalaserene@vit.ac.in*

## Overview

This project introduces a novel approach utilizing hybrid machine learning algorithms to predict start-up success. Acknowledging the inherent risks in the start-up landscape, we aim to demystify the perception of high failure rates associated with new ventures. By combining algorithms such as Logistic Regression, K-Nearest Neighbours, Random Forest, Naive Bayes, Gradient Boosting, and Support Vector Machine, our approach achieves an accuracy of up to 96.22%.

## Keywords

- Logistic Regression
- K-Nearest Neighbours
- Random Forest
- Naïve Bayes
- Gradient Boosting
- Support Vector Machine
- Start-up
- Hybrid Model

## Introduction

Start-ups are newly established businesses focusing on innovative products, services, or business models. These ventures are often perceived as risky due to high failure rates, uncertain market conditions, limited resources, and execution challenges. Our hybrid machine learning model aims to provide a robust prediction of start-up success, assisting investors and stakeholders in making informed decisions.

## Methodology

### Data Pre-processing

- Dropping columns with missing values
- Label encoding categorical features

### Feature Selection

- Using XGBoost to select features with importance scores above 0.1

### Hybrid Model Construction

- Combining Logistic Regression, K-Nearest Neighbours, Random Forest, Naive Bayes, Gradient Boosting, and Support Vector Machine

### Ensemble Model Development

- Using VotingClassifier to combine Gradient Boosting, Random Forest, and SVM

### Evaluation and Visualization

- Calculating accuracy, precision, recall, F1-score, and confusion matrix
- Visualizing results using bar plots, line plots, and heat-maps

## Experimental Setup

### Dataset

- Features: company details, team attributes, market presence, financial indicators, technological focus
- Class imbalance: 64.6% successful, 35.4% unsuccessful
- Addressing imbalance using SMOTE oversampling

### Proposed Architecture

1. Data Acquisition and Pre-processing
2. Feature Selection using XGBoost
3. Hybrid Model Construction
4. Ensemble Model Development
5. Evaluation and Visualization
6. Deployment and Monitoring

### Hardware and Software

- High-performance computing system with multi-core processors
- Software: scikit-learn, XGBoost, TensorFlow, Python, Matplotlib, Seaborn

### Results

| Hybrid Algorithms                        | Accuracy | F1-Score | Precision | Recall  |
|------------------------------------------|----------|----------|-----------|---------|
| Logistic Regression and K-Nearest Neighbours | 93.53%   | 94.77%   | 94.57%    | 94.63%  |
| Random Forest and Naïve Bayes            | 94.58%   | 94.67%   | 94.57%    | 94.43%  |
| Ensemble of Gradient Boosting, Random Forest, and SVM | 96.52%   | 97.67%   | 97.57%    | 97.43%  |

## Figures

### Heatmap of the Dataset

![Heatmap](path/to/heatmap.png)

### Pie Chart Distribution of the Target Variable

![Pie Chart](path/to/piechart.png)

### Correlation Matrix

![Correlation Matrix](path/to/correlationmatrix.png)

### Feature Selection

![Feature Selection](path/to/featureselection.png)

### Algorithmic Flowchart

![Algorithmic Flowchart](path/to/algorithmflowchart.png)

### Architecture Diagram

![Architecture Diagram](path/to/architecturediagram.png)

### Code Output

![Code Output](path/to/codeoutput.png)

### Confusion Matrix

![Confusion Matrix](path/to/confusionmatrix.png)

### Comparing Performance Matrix

![Comparing Performance Matrix](path/to/comparingperformancematrix.png)

## Conclusion

This research demonstrates the potential of hybrid machine learning techniques in predicting start-up success with high accuracy. The ensemble model, combining multiple algorithms, has shown superior predictive performance. Future work could explore additional data sources, further feature engineering, and optimization of model architectures.

## Contributions

- **Conceptualization**: Dhruv Sompura and Priyadarshan Jain
- **Methodology**: Dhruv Sompura
- **Formal Analysis**: Dr. Malaserene
- **Investigation**: Priyadarshan Jain
- **Writing – Review & Editing**: Dhruv Sompura
- **Supervision**: Dr. Malaserene

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

We thank the School of Computer Science Engineering and Information Systems, Vellore Institute of Technology, for their support.

