# OnlineTransactionFraudDetection
Online Transaction Fraud Detection - Machine Learning
Explanation:
Dataset Construction: The data provided is manually structured into a pandas DataFrame to mimic the dataset from the tables you shared.

Train-Test Split: The dataset is split into training and testing sets using train_test_split from sklearn.

Preprocessing:
-Numerical features (step, amount, oldbalanceOrg, newbalanceOrig, etc.) are scaled using StandardScaler.
-Categorical features (type) are encoded using OneHotEncoder.
-Pipeline: A pipeline is used to streamline the preprocessing and modeling process. The ColumnTransformer is used to apply different preprocessing steps to different columns, and then a RandomForestClassifier is used to classify the transactions.

Model Evaluation:
-Classification Report shows precision, recall, and F1-score.
-Confusion Matrix gives a breakdown of the true/false positives and negatives.
-ROC-AUC Score evaluates the model's ability to discriminate between classes.

Notes:
-This code uses a simple dataset. In a real-world scenario, you'd be working with a much larger dataset, so make sure to load your actual dataset.
-Hyperparameter tuning (e.g., adjusting the parameters of the RandomForestClassifier) can be done using tools like GridSearchCV.
The dataset and model pipeline should be tested with more diverse and complex data for better performance.
