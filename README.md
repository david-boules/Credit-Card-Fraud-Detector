# Credit Card Fraud Detector Project
This project focuses on detecting fraudulent credit card transactions using machine learning.

Credit card fraud detection is highly relevant and important in the real world since according to Merchant Cost Consulting, digital transactions represent larger prooprtions of all in-person transactions globally year on year, with cash transactions representing just 16% of all in-person transactions, as of December 2024.
Credit card fraud detection can help prevent financial loss for individual consumers and organizations alike and enhance security in digital transaction systems, which is the motivation for this project.

---

## Dataset Description
### Key Information
The dataset contains transactions made by European cardholders over two days in September of 2013, reaching a total of 284,807 transactions. The data was collected by Wordline and the Machine Learning Group of ULB (Université Libre de Bruxelles)
The dataset was transformed using Principal Component Analysis (PCA) for the purpose of ensuring anonymity in this dataset by hiding identifiable infformation of various credit card users, along with the aim of dimensionality reduction and feature transformation for machine learning pipelines

### Dataset Features
- The dataset is highly imbalanced, where only 492 transactions are fraud, accoutning for only 0.172% of all transactions in this dataset.
- Due to confidentiality requirements, the majority of features do not represent a tangible, physical quantity, as the variables: V1, V2,..., V28 represent 28 variables that are a result of PCA transformation.
- Two infromative features exist: 1) Amount - the transaction amount, 2) Time - the seconds elapsed between each transaction and the first transaction in the dataset

As a result of the massive class imbalance, oversampling and undersampling techniques must be used, either individually or in combination. Additionally, typical measures of 'accuracy' may not be informative, which calls for using other measures such as ROC AUC curve.

---

## Project Timeline
1. **Phase 1**: Exploratory Data Analysis & Statistical Analysis
   - Understand dataset properties (e.g., class imbalance, feature distributions)
   - Perform exploratory data analysis (EDA)
2. **Phase 2**: Preprocessing & Feature Engineering
   - Handle class imbalance using oversampling/undersampling techniques
   - Explore feature importance
3. **Phase 3**: Model Building & Evaluation
   - Train different models (e.g., Logistic Regression, Random Forest, KNN, SVM)
   - Use cross-validation for performance evaluation with metrics like Recall and ROC-AUC
   - Conduct hyperparameter tuning to improve model performance and avoid overfitting (e.g., Grid Search, Random Search, Bayesian Optimization)
4. **Phase 4**: Results Analysis & Insights
   - Compare models based on various metrics
   - Identify trade-offs between false positives and false negatives
   
---

## Future Work
- Explore deep learning models for fraud detection
- Deploy the model as a web application
- Explore a more recent dataset (if available)

---

## References
- [ULB Machine Learning Group](http://mlg.ulb.ac.be)
- [SMOTE Documentation](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)
- [Dataset from Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data)
- [Credit Card Fraud Statistics by Merchant Cost Consulting](https://merchantcostconsulting.com/lower-credit-card-processing-fees/credit-card-fraud-statistics/)

---

## License
This project is licensed under the MIT License. See the LICENSE file for details
