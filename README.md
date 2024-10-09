# Hotel Cancellation Prediction
Project Overview
This project aims to predict if a customer will cancel their hotel booking or not. Accurately forecasting cancellations helps hotels manage bookings more effectively, reducing the financial impact of last-minute cancellations and optimizing resource allocation.

Workflow Summary
Data Preprocessing
One-Hot Encoding: Categorical variables were transformed into numerical form using one-hot encoding to make the data compatible with machine learning algorithms.
Outlier Handling: Outliers were managed using the Z-score method to improve model robustness and prevent skewed predictions.
Feature Selection: Only the most relevant features were selected to streamline the model and enhance performance.
Model Development
Hyperparameter Tuning: The model's hyperparameters were optimized using RandomizedSearchCV to identify the best configuration for the RandomForestClassifier.
Random Oversampling: To address class imbalance (since cancellations are less frequent than non-cancellations), random oversampling was applied to balance the dataset.
Random Forest Classifier: The RandomForestClassifier was chosen for its strong predictive capabilities, especially when dealing with both categorical and numerical data. It also provides insights into feature importance, helping understand what factors influence cancellations.
Cross-Validation: Cross-validation was applied to the training dataset to evaluate model performance and ensure it generalizes well to unseen data.
Results
The model achieved an accuracy of 94% on the test set, demonstrating high accuracy in predicting whether a customer will cancel their booking or not.
Model Saving
The trained model was saved using the pickle library, enabling easy reloading and use in production environments.
