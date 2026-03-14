# 🏠 Housing Price Prediction using Machine Learning

## 📌 Project Overview

This project builds a **machine learning model to predict housing prices** using a housing dataset. The notebook demonstrates a complete **end-to-end machine learning workflow**, including data exploration, preprocessing, feature engineering, model training, evaluation, and hyperparameter tuning.

The goal is to learn how to transform raw housing data into a **predictive regression model** capable of estimating house values based on different features.

This project is a practical example of applying **data science and machine learning techniques using Scikit-learn**.

---

# 📊 Dataset

The dataset contains information about houses and their characteristics. It includes numerical and categorical variables describing each property.

### Example Features

Typical attributes in the dataset include:

* `longitude` – Geographic longitude
* `latitude` – Geographic latitude
* `housing_median_age` – Median age of houses
* `total_rooms` – Total number of rooms
* `total_bedrooms` – Total number of bedrooms
* `population` – Population in the area
* `households` – Number of households
* `median_income` – Median income of residents
* `ocean_proximity` – Distance from the ocean (categorical)
* `median_house_value` – Target variable (house price)

The goal is to predict **median house value** using the other features.

---

# ⚙️ Technologies Used

The project uses the following tools and libraries:

* **Python**
* **Pandas** – Data manipulation
* **NumPy** – Numerical computing
* **Matplotlib & Seaborn** – Data visualization
* **Scikit-learn** – Machine learning models
* **Joblib** – Model saving/loading
* **Jupyter Notebook** – Development environment

---

# 🔎 Exploratory Data Analysis (EDA)

The project begins with data exploration to understand patterns and relationships.

EDA tasks include:

* Dataset overview
* Summary statistics
* Correlation analysis
* Scatter matrix visualization
* Geographic price visualization

These steps help identify **important features influencing house prices**.

---

# 🧹 Data Preprocessing

Before training the model, the data is cleaned and transformed.

Key preprocessing steps include:

### Handling Missing Values

Missing numerical values are handled using appropriate imputation strategies.

### Feature Scaling

Numerical features are standardized using:

* **StandardScaler**

### Encoding Categorical Variables

The `ocean_proximity` categorical feature is converted into numerical values using:

* **OneHotEncoder**

### Feature Engineering

Additional features may be created to improve model performance.

---

# 🔧 Machine Learning Pipeline

A **Scikit-learn pipeline** is created to automate preprocessing and model training.

Pipeline steps include:

1. Numerical feature scaling
2. Categorical feature encoding
3. Model training

Using pipelines ensures that the same preprocessing steps are consistently applied to both training and testing data.

---

# 🤖 Models Used

Several regression models are trained and compared:

### Linear Regression

A baseline model for predicting house prices.

### Decision Tree Regressor

Captures nonlinear relationships in the data.

### Random Forest Regressor

An ensemble learning method that improves prediction accuracy by combining multiple decision trees.

---

# ⚡ Model Evaluation

Models are evaluated using regression metrics such as:

* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**
* **R² Score**

Cross-validation is used to measure how well the models generalize to unseen data.

---

# 🔍 Hyperparameter Tuning

To improve model performance, **GridSearchCV** is used to find the best parameters for the Random Forest model.

Parameters tuned may include:

* Number of trees (`n_estimators`)
* Maximum depth
* Maximum number of features

This process helps select the **optimal model configuration**.

---

# 📈 Project Workflow

```
Data Collection
       ↓
Exploratory Data Analysis
       ↓
Data Cleaning & Preprocessing
       ↓
Feature Engineering
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Hyperparameter Tuning
       ↓
Final Model Selection
```

---

# 📂 Project Structure

```
housing-price-prediction
│
├── housing.ipynb          # Main notebook with ML workflow
├── housing.csv            # Housing dataset
├── model.joblib           # Saved trained model (optional)
├── README.md              # Project documentation
└── requirements.txt       # Python dependencies
```

---

# 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```
git clone https://github.com/-Housing-Price/housing-price-ml.git
```

### 2️⃣ Navigate to the Project Folder

```
cd housing-price-ml
```

### 3️⃣ Install Dependencies

```
pip install -r requirements.txt
```

### 4️⃣ Run the Notebook

```
jupyter notebook
```

Open the notebook and run the cells step-by-step.

---

# 🔮 Future Improvements

Possible enhancements for this project:

* Deploy the model with **FastAPI or Flask**
* Build a **web app for price prediction**
* Use **XGBoost or Gradient Boosting models**
* Add **feature importance visualization**
* Create a **real-time prediction API**

---

# 👨‍💻 Author

This project was developed as part of a **machine learning learning journey** to practice building end-to-end regression models using Scikit-learn and real-world housing datasets.
