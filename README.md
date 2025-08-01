# Summer-Final-Project
This project uses U.S. Census data to build a machine learning model that predicts whether an individual earns over $50K per year based on their demographic and work-related attributes. The goal is to explore the full ML pipeline - from preprocessing to evaluation - using models like Logistic Regression and Random Forest.

🧹 Data Preprocessing

Feature Selection: Retained key numerical features like age, education-num, capital-gain, capital-loss, and hours-per-week.

Categorical Encoding: Applied one-hot encoding to variables like workclass, education, marital-status, occupation, relationship, race, sex, and native country.

Handling Missing Data: Imputed missing values using SimpleImputer with median (numeric) and most frequent (categorical) strategies.

Outlier Treatment: Applied winsorization to capital-gain and capital-loss to cap extreme values at the 1st and 99th percentiles.

Feature Scaling: Standardized numeric features using StandardScaler to ensure equal weighting across features.

⚙️ Models Used

Logistic Regression
Random Forest 
Classifier (with GridSearchCV for hyperparameter tuning)

📈 Model Evaluation

Models were assessed using the following metrics:

Accuracy
Precision
Recall
F1-Score
ROC AUC Score
Confusion Matrix

The Random Forest model outperformed logistic regression, especially in correctly identifying higher-income individuals.

📌 Key Insights

Class imbalance significantly impacted model performance on the minority class (>50K).

Feature importance analysis revealed that education-num, hours-per-week, and capital-gain were among the top predictors.

Winsorizing outliers improved model stability.

Standard scaling helped improve convergence for Logistic Regression.

