# 1.0 Business Problem
Blocker Fraud Company specializes in detecting fraud in financial transactions made through mobile devices. Their service, "Blocker Fraud," guarantees the blocking of fraudulent transactions. The company has adopted an aggressive strategy to acquire customers, where they earn revenue based on successful fraud detection. However, they also bear the risk of reimbursing customers in case of false positives. The goal is to build accurate models to maximize revenue while minimizing losses.

## 2.0 Business Assumptions
- Fraud prevention is crucial to avoid financial damage and protect the reputation of clients and financial institutions.
- Financial frauds can occur through virtual and physical means.

## 3.0 Solution Strategy
The solution involves developing a data science project with a machine learning model to predict whether a transaction is fraudulent. The process is broken down into several steps:

### Data Description
- Collect and study data, handle missing values, and calculate descriptive statistics.

### Feature Engineering
- Create a mind map to generate hypotheses and new features.

### Data Filtering
- Remove irrelevant columns or rows not contributing to the business.

### Exploratory Data Analysis
- Conduct univariate, bivariate, and multivariate analyses to understand the data.

### Data Preparation
- Transform data for machine learning, including encoding, oversampling, subsampling, or rescaling.

### Feature Selection
- Use algorithms like Boruta to select the best columns and reduce dimensionality.

### Machine Learning Modeling
- Train and validate machine learning algorithms using cross-validation.

### Hyperparameter Fine Tuning
- Fine-tune the parameters of the selected model for improved performance.

### Conclusions
- Test the model's generalization capacity with unseen data and answer business questions.

### Model Deploy
- Create a Flask API and save the model for deployment.

## 4.0 Top 3 Data Insights
1. All fraud amounts are greater than 10,000.
2. 60% of fraud transactions occur using the cash-out method.
3. Values greater than 100,000 occur mainly using the transfer method.

## 5.0 Machine Learning Applied
Cross-validation results for different models:

- Dummy Model
- Logistic Regression
- K Nearest Neighbors
- Support Vector Machine
- Random Forest
- XGBoost
- LightGBM

## 6.0 Machine Learning Performance
The chosen model is XGBoost with tuned parameters, providing the following performance:

- Balanced Accuracy: 88.1%
- Precision: 96.3%
- Recall: 76.3%
- F1 Score: 85.1%
- Kappa: 85.1%

## 7.0 Business Results
- The company can earn approximately R$ 60,613,782.88 detecting true fraud transactions.
- Revenue for detecting fraud transactions that are legitimate is estimated at R$ 183,866.98.
- The company needs to refund R$ 3,546,075.42 for legitimate transactions classified as fraud.
- Precision and accuracy for unseen data are 94.4% and 91.5%, respectively.
- The model can detect 82.9% of fraud in unseen data.

## 8.0 Conclusions
Despite extreme class imbalance, it's possible to create a model with good scores. The company can expect a significant revenue increase using the developed model.

## 9.0 Lessons Learned
- Unbalanced classes can be addressed effectively with proper modeling techniques.
- Models can be created to classify classes with less than 1% of samples.
