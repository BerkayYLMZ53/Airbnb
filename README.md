# 🗺️ Airbnb User Booking Prediction (Term Project)

This project was developed to predict which country new Airbnb users will make their first booking in by analyzing their demographic data, location preferences, and session activity. It is an end-to-end machine learning study based on a multi-class classification problem.

## 🎯 Project Objective
To predict users' travel destinations beforehand in order to personalize the user experience, highlight popular content related to the respective destination, and direct marketing budgets toward the appropriate target audience.

## 📊 Dataset Structure and Preprocessing
The dataset used in this project includes user profile information and in-app interactions. The following steps were implemented during the data preprocessing phase:
* **Missing Value Management:** Missing and incomplete data in the dataset were analyzed and either cleaned or imputed using appropriate methods.
* **Categorical Variable Transformation:** Categorical metrics were prepared for the models using `LabelEncoder` and `One-Hot Encoding` methods.
* **Feature Scaling:** `StandardScaler` was applied to balance the impact of continuous variables on the models.

## 🛠️ Technologies and Models Used
The project utilizes the Python programming language along with libraries from its data science ecosystem, including `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, and `Scikit-Learn`.

Three different algorithms were evaluated and compared to find a suitable approach:
1. **Logistic Regression:** To measure baseline linear classification performance.
2. **Random Forest Classifier:** To observe ensemble learning performance.
3. **Gradient Boosting Classifier:** To optimize weak learners using gradient boosting to achieve higher accuracy.

## 📈 Hyperparameter Optimization and Results
To improve model performance, hyperparameter combinations were selected using **`RandomizedSearchCV`** and **`GridSearchCV`**.

* **Best Performing Model:** `Gradient Boosting Classifier`
* **Evaluation:** Model performance was evaluated using accuracy, precision, recall, and F1-score metrics, which are critical for multi-class classification problems.
* **Visualization:** A detailed **Confusion Matrix** heatmap (`sns.heatmap`) was generated to analyze where the optimized model made correct and incorrect predictions across different countries.

## 🚀 Running the Project Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/BerkayYLMZ5353/airbnb-booking-prediction.git
   ```
