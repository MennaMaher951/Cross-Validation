## Heart Disease Prediction with Cross-Validation
* This project explores the prediction of heart disease using various machine learning models and leverages cross-validation for robust performance evaluation. We use the "heart disease" dataset for our analysis.

*Methodology*

* Data Acquisition and Preprocessing:
1. Load the dataset using pandas.
2. Perform initial data exploration and analysis.
3. Separate features and the target variable ("target").
4. Perform a stratified train-test split to ensure balanced class distribution.

* Models Training and Evaluation:
* Train four machine learning models: Logistic Regression, SVC (linear kernel), KNeighborsClassifier, and RandomForestClassifier.
* Evaluate models performance on the test set using accuracy score.
* Implement 5-fold cross-validation to obtain a more reliable estimate of model generalization.

* Results and Discussion:
* Both Logistic Regression and SVC achieve similar mean accuracy of around 82.83% on both the test set and cross-validation, indicating good performance.
* Random Forest Classifier comes in close behind with a mean accuracy of 80.85% on cross-validation.
* KNeighborsClassifier performs the worst with a mean accuracy of 64.39% on cross-validation, suggesting limitations for this dataset.

* Conclusion:
1. Based on the results, Logistic Regression and SVC are suitable models for predicting heart disease in this dataset, demonstrating consistent performance across both standard evaluation and cross-validation.
2. Further exploration could involve hyperparameter tuning for each model, exploring other algorithms, and evaluating on an independent dataset for generalizability.

*Cross-Validation Importance*
* Cross-validation is crucial in machine learning to avoid overfitting and obtain a realistic estimate of model performance on unseen data. By repeatedly splitting the data into training and validation sets and averaging the results, we gain a more robust understanding of how well a model will generalize to new data.

* Dependencies
1. pandas
2. numpy
3. scikit-learn
