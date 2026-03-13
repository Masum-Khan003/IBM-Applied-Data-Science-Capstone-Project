# 🚀 Falcon 9 Landing Success Prediction

### Applied Data Science Capstone Project

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Visualization](https://img.shields.io/badge/Data%20Visualization-Plotly%20%7C%20Seaborn-green)
![Database](https://img.shields.io/badge/Database-IBM%20DB2-blueviolet)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

# 📌 Project Overview

SpaceX dramatically reduced the cost of space launches by **reusing the Falcon 9 rocket’s first-stage booster**.
A Falcon 9 launch costs approximately **$62 million**, whereas other providers may charge **$165 million or more**.

The **key determinant of this cost advantage is whether the first stage lands successfully** and can be reused.

This project applies **data science and machine learning techniques** to predict the landing success of Falcon 9 boosters using historical launch data.

The work demonstrates a **complete end-to-end data science workflow**, including:

* Data collection from APIs and web scraping
* Data cleaning and transformation
* Exploratory data analysis
* Feature engineering
* Interactive visual analytics
* Machine learning model development and optimization

Such predictive insights can help organizations **estimate launch costs and compete with SpaceX in the commercial launch market**.

---

# 🎯 Project Objectives

The project aims to:

* Collect and integrate **real-world launch data**
* Perform **exploratory data analysis (EDA)** to identify key patterns
* Engineer features that influence landing outcomes
* Build **interactive dashboards** for data exploration
* Train and optimize **machine learning models**
* Evaluate models to determine the best predictor of landing success

---

# 📊 Data Sources

### 1️⃣ SpaceX REST API

Provides historical Falcon 9 launch data including:

* Launch site
* Booster version
* Payload mass
* Orbit type
* Launch outcomes

### 2️⃣ Wikipedia Falcon 9 Launch Records

Additional mission records were collected through **web scraping** to enrich the dataset.

---

# 🧠 Data Science Pipeline

```
Data Collection
      │
      ▼
Data Wrangling & Cleaning
      │
      ▼
Exploratory Data Analysis (EDA)
      │
      ▼
Feature Engineering
      │
      ▼
Database Integration (SQL)
      │
      ▼
Interactive Visualization (Dash)
      │
      ▼
Machine Learning Models
      │
      ▼
Model Evaluation
```

---

# ⚙️ Methodology

## 1️⃣ Data Collection & Wrangling

* Retrieved launch data using **SpaceX API requests**
* Converted JSON responses into structured datasets
* Cleaned missing values and standardized formats
* Prepared the dataset for analysis

---

## 2️⃣ Web Scraping

Launch records were extracted from Wikipedia using:

* **BeautifulSoup**
* HTML table parsing
* Conversion into **Pandas DataFrames**

This provided additional historical data to complement the API dataset.

---

## 3️⃣ Exploratory Data Analysis (EDA)

EDA was performed using:

* **Matplotlib**
* **Seaborn**

The analysis explored relationships between:

* Launch site and success rate
* Payload mass and landing outcomes
* Orbit type and mission success
* Booster versions and reliability

These insights guided **feature engineering and model selection**.

---

## 4️⃣ Database Integration

The dataset was loaded into an **IBM Db2 database** to enable structured analysis using SQL.

Examples of analysis performed:

* Launch success by site
* Mission frequency by orbit
* Payload mass distribution

This step demonstrates **integration of SQL with data science workflows**.

---

## 5️⃣ Feature Engineering & Geospatial Visualization

New features were engineered to improve model performance.

Geospatial analysis was performed using **Folium**, enabling:

* Interactive maps of launch sites
* Visualization of success vs failure
* Geographic patterns in launch outcomes

---

## 6️⃣ Interactive Data Analytics Dashboard

An interactive dashboard was built using **Plotly Dash**.

### Key Features

* Launch site selection
* Payload mass filtering
* Interactive pie charts
* Scatter plot analysis of launch outcomes

This application allows users to **explore mission data dynamically**.

---

# 🤖 Machine Learning Models

The project trained several classification models to predict **first-stage landing success**.

### Data Preparation

* Feature scaling using **StandardScaler**
* Train/Test split for model evaluation

### Models Implemented

* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree Classifier
* K-Nearest Neighbors (KNN)

### Hyperparameter Optimization

Model tuning was performed using:

**GridSearchCV**

to identify optimal parameters.

---

# 📈 Model Performance

| Model                    | Test Accuracy       |
| ------------------------ | ------------------- |
| Decision Tree Classifier | **0.9444**          |
| Support Vector Machine   | 0.8333              |
| K-Nearest Neighbors      | 0.8333              |
| Logistic Regression      | Comparable baseline |

### 🏆 Best Performing Model

The **Decision Tree Classifier** achieved the highest accuracy of:

**94.44%**

making it the most effective model for predicting Falcon 9 landing success in this study.

---

# 📊 Technologies Used

### Programming

* Python

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn
* Plotly
* Folium

### Machine Learning

* Scikit-learn

### Data Collection

* SpaceX REST API
* BeautifulSoup (Web Scraping)

### Database

* IBM Db2
* SQL

### Interactive Dashboard

* Plotly Dash

---

# 📁 Repository Structure

```
Falcon9-Landing-Prediction
│
├── data/
│   ├── raw datasets
│   ├── cleaned datasets
│
├── notebooks/
│   ├── Data collection
│   ├── EDA
│   ├── Feature engineering
│   ├── Machine learning models
│
├── scripts/
│   ├── preprocessing
│   ├── modeling scripts
│
├── dash_app/
│   ├── Plotly Dash dashboard
│
└── README.md
```

---

# 💡 Key Insights

* Launch site location significantly influences landing success.
* Payload mass affects recovery probability.
* Certain booster versions demonstrate higher landing reliability.
* Machine learning models can successfully learn patterns from historical launch data.

---

# 🔮 Future Improvements

Potential future enhancements include:

* Adding **new SpaceX launch data**
* Testing **ensemble models (Random Forest, XGBoost)**
* Deploying the dashboard as a **web application**
* Integrating **real-time launch data pipelines**

---

# 🎓 Project Context

This project was completed as part of the:

**IBM Applied Data Science Professional Certificate**

on **Coursera**.

It serves as a **capstone project demonstrating practical data science skills**, including data engineering, analysis, machine learning, and interactive visualization.

---

# ⭐ If you find this project interesting

Feel free to explore the notebooks and the interactive dashboard included in this repository.

Contributions, suggestions, and feedback are always welcome.
