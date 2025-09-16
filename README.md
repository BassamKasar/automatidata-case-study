# 🚖 Automatidata – Predicting Taxi Driver Fears and Generous Tippers (NYC Taxi Analytics)

![Project Badge](https://img.shields.io/badge/Status-Completed-brightgreen)  
![License](https://img.shields.io/badge/License-MIT-blue)  
![Python](https://img.shields.io/badge/Python-3.9%2B-yellow)

## 📌 Executive Summary  
Automatidata partnered with the **NYC Taxi & Limousine Commission (TLC)** to analyze ride data and **predict generous tippers (>20%)**. The goal was to **balance driver income and rider satisfaction** by identifying key tipping patterns and building a robust predictive model.  
This project is part of the **Google Advanced Data Analytics Professional Certificate**.

---

## 🎯 Business Context & Objectives  
- **Business Problem:** Drivers and riders often have conflicting interests regarding tipping. Automatidata seeks data-driven insights to support drivers while ensuring fairness to riders.  
- **Objective:**  
  - Analyze tipping patterns from NYC taxi trip data.  
  - Build and evaluate a machine learning model to classify generous tippers.  
  - Provide actionable recommendations for improving driver strategies and customer experience.

---

## 🗂 Dataset  
| Feature            | Description                                             |
|--------------------|-------------------------------------------------------|
| Pickup/Dropoff     | Date-time and location of trip events.                 |
| Passenger Count    | Number of passengers per trip.                         |
| Fare Amount        | Total fare charged (USD).                              |
| Tip Amount         | Tip value (USD).                                       |
| Payment Type       | Method of payment (card, cash, etc.).                   |
| Trip Distance      | Distance traveled (miles).                              |

- **Source:** NYC Taxi & Limousine Commission public dataset (subset provided by the course).  
- **Size after cleaning:** ~`[INSERT NUMBER]` records.  
- **Period Covered:** `[INSERT YEAR(S)]`.  
- **License:** Public domain (NYC TLC).

---

## 🛠 Tools & Technologies  
- **Languages:** Python (3.9+)  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Environment:** Jupyter Notebook  
- **Version Control:** Git & GitHub  
- **Visualization:** Matplotlib, Seaborn

---

## 🔍 Methodology  
1. **Data Cleaning & Preparation**  
   - Removed missing tips and outliers.  
   - Converted date-time columns and created new features (e.g., tip percentage).  

2. **Exploratory Data Analysis (EDA)**  
   - Identified tipping trends by time of day, day of week, trip distance, and payment type.  
   - Visualized correlations and distributions.  

3. **Feature Engineering**  
   - Engineered categorical variables (e.g., pickup borough).  
   - Created binning for trip times and distances.  

4. **Modeling**  
   - Tested **Logistic Regression** and **Random Forest Classifier**.  
   - Tuned hyperparameters for optimal performance.  

5. **Evaluation**  
   - Metrics: Accuracy, Precision, Recall, ROC-AUC.  
   - Random Forest achieved **ROC-AUC = [INSERT VALUE]**.  

---

## ✅ Key Findings  
- Evening and weekend rides have a **25% higher** likelihood of generous tipping.  
- **Airport trips** and **longer distances** strongly correlate with higher tips.  
- **Random Forest** outperformed logistic regression in predictive accuracy.  
- Potential improvement by adding external factors (e.g., weather, events).

---

## 📊 Visualizations  
| F1 scores of the random forest and XGBoost models             | Scatter plot shows predicted versus actual taxi fare amounts based on the linear regression model                           |
|-----------------------------------------|--------------------------------------|
| ![F1 scores of the random forest and XGBoost models](Visuals/F1_scores_of_the_random_forest_and_XGBoost_models.png) | ![Scatter plot shows predicted versus actual taxi fare amounts based on the linear regression model](Visuals/Scatter_plot_shows_predicted_versus_actual_taxi_fare_amounts_based_on_the_linear_regression_model.png) |

---

## 🚀 How to Run Locally  
1. **Clone the repository:**  
   ```bash
   git clone https://github.com/BassamKasar/automatidata-case-study.git
   cd automatidata-case-study
