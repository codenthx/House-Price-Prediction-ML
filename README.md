🏠 House Price Prediction using Machine Learning

<p align="center">
  <b>A complete supervised machine learning regression project to predict residential house prices using multiple ML algorithms, model evaluation, cross-validation, and hyperparameter tuning.</b>
</p>---

📌 Project Overview

Buying a house involves many factors such as location, quality, size, age, and facilities. This project explores how machine learning can learn patterns from historical housing data and predict house prices.

The goal was not only to build a prediction model, but to follow a complete professional machine learning workflow:

Data → Analysis → Modeling → Evaluation → Optimization → Deployment Ready Model

---

🎯 Objective

Build and compare multiple supervised learning regression models to predict house sale prices and identify the best-performing algorithm.

---

📂 Dataset

Dataset: Kaggle House Prices - Advanced Regression Techniques
Dataset source:

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

The dataset contains detailed information about residential properties including:

- 🏡 Overall quality
- 📐 Living area
- 🛏 Number of rooms
- 🚗 Garage features
- 📍 Neighborhood information
- 🏗 Year built
- 🔧 Property characteristics

Target Variable

SalePrice

The model learns relationships between house features and final selling prices.

---

🔬 Machine Learning Pipeline

                Dataset
                   |
                   ↓
        Exploratory Data Analysis
                   |
                   ↓
          Feature / Target Split
                   |
                   ↓
          Train-Test Split
                   |
                   ↓
        Multiple ML Algorithms
                   |
                   ↓
       Cross Validation Evaluation
                   |
                   ↓
       Hyperparameter Optimization
                   |
                   ↓
          Final Model Selection

---

🤖 Models Implemented

1. Linear Regression

A baseline regression algorithm that learns linear relationships between input features and house prices.

---

2. Decision Tree Regressor 🌳

A tree-based model capable of learning complex non-linear patterns in housing data.

---

3. K-Nearest Neighbors (KNN) Regressor

A distance-based algorithm that predicts prices using similar houses from the dataset.

Hyperparameter tuning was performed to find the optimal number of neighbors.

Best parameter:

K = 7

---

4. Support Vector Regression (SVR)

A regression approach based on Support Vector Machines.

The model was tested and compared with other algorithms.

---

📊 Evaluation Metrics

Models were evaluated using:

Metric| Description
MAE| Average prediction error
MSE| Penalizes larger mistakes
RMSE| Prediction error in price units
R² Score| Amount of variance explained by the model

---

🏆 Model Performance

Model| R² Score
🌳 Decision Tree| 0.7955
KNN| 0.7285
Linear Regression| 0.6555
SVR| -0.0245

---

🥇 Final Model Selection

Decision Tree Regressor

The Decision Tree achieved the best performance among tested algorithms.

Why it performed well:

- Captures non-linear relationships
- Learns complex feature interactions
- Handles varied housing patterns effectively

The trained model was saved using:

joblib

and stored inside:

models/

---

🧪 Model Validation

Cross Validation

5-Fold Cross Validation was performed to ensure the model evaluation was reliable instead of depending on a single train-test split.

Benefits:

✅ More reliable performance estimation
✅ Reduced dependency on one random split
✅ Better understanding of model stability

---

⚙️ Hyperparameter Tuning

GridSearchCV was used to optimize model parameters.

Example:

For KNN:

Tested:

K = 3
K = 5
K = 7
K = 9
K = 11

Best value:

K = 7

---

📁 Project Structure

House_Price_Prediction/

│
├── data/
│   └── Dataset files
│
├── notebook/
│   └── Machine Learning notebook
│
├── images/
│   └── EDA and visualization graphs
│
├── models/
│   └── Saved trained models
│
├── reports/
│   └── Evaluation results
│
├── README.md
│
└── requirements.txt

---

🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Google Colab

---

📚 Key Concepts Learned

Through this project:

- Supervised Learning
- Regression Problems
- Feature and Target Separation
- Train-Test Split
- Cross Validation
- Bias vs Variance
- Model Evaluation
- Hyperparameter Tuning
- Model Comparison

---

🚀 Future Improvements

Possible improvements:

- Feature engineering
- Handling categorical variables with advanced encoding
- Ensemble models:
  - Random Forest
  - Gradient Boosting
  - XGBoost
- Deployment using Flask/FastAPI
- Creating a web interface for predictions

---

👩‍💻 Author

Amna Faisal

Electrical Engineering Student
Machine Learning Internship Project

---

⭐ If you found this project useful, consider giving it a star!