# Verizon Customer Default Prediction

This script analyzes Verizon customer data to predict customer defaults. It performs exploratory data analysis (EDA), visualizes key relationships between variables, and builds two machine learning models for classification: Logistic Regression and Random Forest.

## Key Steps:

1. **Data Exploration & Visualization**:
   - Load and inspect the dataset.
   - Check for missing values and visualize them.
   - Explore the distribution of defaults and key features, including gender, age, payment type, down payment, credit score, and price.
   - Visualize correlations between features like `price`, `downpmt`, and `credit_score`.

2. **Preprocessing**:
   - Drop the target column `default` for feature selection.
   - Split the dataset into training and test sets (60% training, 40% testing).
   - Standardize the features using `StandardScaler`.

3. **Model Building & Evaluation**:
   - Build a **Logistic Regression** model and a **Random Forest** model to predict the likelihood of default.
   - Evaluate both models using confusion matrices and classification reports, showing key metrics like precision, recall, and F1-score.

4. **Feature Importance**:
   - For the Random Forest model, plot the feature importances to highlight which features have the most influence on predicting defaults.

## Libraries Used:
- `pandas`: Data manipulation and analysis
- `matplotlib` and `seaborn`: Data visualization
- `sklearn`: Machine learning model building and evaluation
