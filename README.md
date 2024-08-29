# Predicting Flight Delay Types
# Overview

This project focuses on predicting the type of flight delays (Top 3: CarrierDelay, LateAircraftDelay, NASDelay) using 2 machine learning classification models. The analysis involves data preprocessing, feature engineering, model training, and evaluation using various classification techniques, Random Forest and Logistic Regression.

# Dataset
The dataset used is the first 500k rows of the total complete dataset contains flight-related information, including attributes such as the month, day of the month, day of the week, departure and arrival times, carrier, origin, destination, distance, taxi-in and taxi-out times, and delays due to different reasons. The target variable is the delay type ('DelayType') derived from the maximum delay among CarrierDelay, LateAircraftDelay, and NASDelay.
https://data.world/data-society/airlines-delay

# Objectives
- EDA: Perform Exploratory Data Analysis to understand feature distributions, relationships, and potential data quality issues.
- Feature Engineering: Create new features, such as departure hour, arrival hour, and indicators for morning and evening flights, to improve model performance.
- Modeling: Apply and compare different classification models, including Random Forest and Logistic Regression, to predict flight delay types.
- Model Evaluation: Evaluate model performance using metrics such as accuracy, precision, recall, and F1-score to identify the best model.

# Methods
- EDA: Conducted exploratory analysis to visualize the distribution of key features and their relationship with the target variable, including checking for missing values.
- Feature Engineering: Added new features like DepTime_hour, ArrTime_hour, Is_Morning_Flight, and Is_Evening_Flight to enhance model prediction power. One-Hot Encoding (OHC) was used to encode categorical variables.
- Modeling: Implemented Random Forest and Logistic Regression classifiers. Hyperparameter tuning for the Random Forest model was performed using RandomizedSearchCV to optimize parameters such as the number of estimators, maximum depth, and minimum samples split.
- Model Evaluation: Compared models using accuracy, precision, recall, and F1-score to determine the most effective model for predicting flight delay types.

# Results
- The Random Forest model achieved an accuracy of 80.43%, demonstrating better performance across all delay categories compared to Logistic Regression.
- Logistic Regression achieved a lower accuracy of 68.54%, indicating that it was less effective in correctly identifying the delay types, especially for 'LateAircraftDelay' and 'NASDelay'.
- The Random Forest model showed a balanced performance with higher precision and recall for all classes, making it the preferred choice.

# Conclusion
- The project highlights the effectiveness of using machine learning techniques, particularly Random Forest, in predicting flight delay types. The feature engineering and model tuning strategies employed contributed significantly to improving the model's accuracy and reliability.
-  The Random Forest model emerged as the best performer and is recommended for deployment in scenarios requiring accurate prediction of flight delays with multiple features.
