# 🏠 House Price Prediction using Machine Learning

Predict house prices in Bengaluru using a complete machine learning pipeline, including data preprocessing, feature engineering, outlier removal, model training, hyperparameter tuning, and model deployment artifacts.

---

## 📌 Project Overview

Real estate prices depend on several factors such as location, area, number of bedrooms, bathrooms, and other property characteristics. Estimating the correct market value manually can be difficult because relationships between these features are often non-linear and influenced by multiple variables.

This project builds a complete Machine Learning pipeline capable of predicting house prices in Bengaluru based on historical housing data. The project covers every major stage of an ML workflow—from raw data preprocessing to training and exporting a production-ready model.

---

# 🎯 Objectives

- Predict house prices accurately using machine learning.
- Clean noisy real-world housing data.
- Perform feature engineering and encoding.
- Remove statistical outliers.
- Compare multiple regression algorithms.
- Select the best-performing model.
- Save the trained model for deployment.
- Build a reusable prediction pipeline.

---

# 🚀 Features

- Complete data preprocessing pipeline
- Missing value handling
- Feature engineering
- One-Hot Encoding
- Outlier detection and removal
- Multiple regression models
- Hyperparameter tuning
- Model serialization using Pickle
- JSON feature mapping
- Predict prices for new houses

---

# 📂 Project Structure

```
House-Price-Prediction-Using-Machine-Learning/
│
├── house-price-prediction-model.ipynb
├── house.py
├── bengaluru_house_prices.csv
├── house_cleaned.csv
├── bhp.csv
├── banglore_home_prices_model.pickle
├── columns.json
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 📊 Dataset

The project uses the Bengaluru House Price Dataset.

Each record contains information such as

- Area (Square Feet)
- Location
- Number of Bedrooms (BHK)
- Number of Bathrooms
- Price

The dataset contains several inconsistencies including

- Missing values
- Incorrect area values
- Rare locations
- Price outliers
- Duplicate-like entries

These issues are handled during preprocessing.

---

# 🧹 Data Preprocessing

The following preprocessing steps are performed:

- Remove unnecessary columns
- Handle missing values
- Clean location names
- Convert area values into numeric format
- Reduce rare locations into an "Other" category
- Remove invalid records
- Create numerical features
- Encode categorical variables

---

# ⚙️ Feature Engineering

Important engineered features include

- Total Square Feet
- Price Per Square Foot
- Location Encoding
- BHK
- Bathrooms

Feature engineering significantly improves model performance.

---

# 📈 Outlier Detection

Real estate datasets usually contain abnormal records.

Examples include

- Extremely expensive houses
- Very small houses with huge prices
- Unrealistic BHK configurations

Outliers are removed using statistical analysis including

- Price per Square Foot filtering
- Standard Deviation method
- Domain-specific rules

---

# 🤖 Machine Learning Models

Several regression algorithms can be evaluated during the project, including:

- Linear Regression
- Lasso Regression
- Decision Tree Regressor

Cross-validation is used to compare performance and select the best model.

---

# 🔍 Hyperparameter Tuning

GridSearchCV is used to search for the best model parameters.

Benefits include

- Improved generalization
- Better prediction accuracy
- Automated model selection

---

# 💾 Model Serialization

After training, the best model is saved using Pickle.

```
banglore_home_prices_model.pickle
```

The feature column names are stored separately in

```
columns.json
```

These files allow predictions without retraining the model.

---

# 📊 Workflow

```
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Missing Value Handling
      │
      ▼
Feature Engineering
      │
      ▼
Outlier Removal
      │
      ▼
Encoding
      │
      ▼
Train-Test Split
      │
      ▼
Model Training
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Best Model Selection
      │
      ▼
Model Serialization
      │
      ▼
Price Prediction
```

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Pickle
- JSON
- Jupyter Notebook

---


# ▶️ Running Predictions

Run

```bash
python house.py
```

The trained model will load automatically and predict house prices based on the provided input.

---

# 📈 Machine Learning Concepts Demonstrated

- Supervised Learning
- Regression
- Data Cleaning
- Feature Engineering
- One-Hot Encoding
- Outlier Detection
- Cross Validation
- Hyperparameter Tuning
- Model Evaluation
- Model Serialization

---

# 📊 Evaluation Metrics

Typical regression metrics include

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

These metrics help compare model performance and estimate prediction accuracy.

---

# 🔮 Future Improvements

- Streamlit Web Application
- Flask REST API
- Docker Deployment
- Model Monitoring
- Automatic Retraining
- Support for Multiple Cities
- Feature Importance Visualization
- Interactive Dashboard

---

# 📚 Learning Outcomes

This project demonstrates practical understanding of

- End-to-end Machine Learning pipeline
- Regression algorithms
- Data preprocessing
- Statistical outlier detection
- Model selection
- Feature engineering
- Model deployment fundamentals

---

# 👨‍💻 Author

**Rhydham Shah**

B.Tech Computer Engineering

Machine Learning | Artificial Intelligence | Competitive Programming

---

## ⭐ If you found this project useful, consider starring the repository!