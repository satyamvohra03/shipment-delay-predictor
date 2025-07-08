# Shipment Delay Predictor 🚚

A machine learning project to predict whether a shipment will be delayed based on historical logistics data.

## 🔧 Tech Stack
- Python (pandas, scikit-learn)
- Jupyter Notebook
- Data Visualization (matplotlib, seaborn)
- Git + GitHub

## 📁 Project Structure


shipment-delay-predictor/
├── data/ # Dataset CSV file
├── notebooks/ # Jupyter notebooks (EDA, model training)
├── models/ # Saved models (optional)
└── README.md # Project overview and instructions



## 🎯 Problem Statement
Build a binary classifier to predict shipment delays using origin, destination, SLA, date patterns, and distance-based features.

## 📊 Features (in dataset)
- Origin & destination hubs
- SLA threshold (in hours)
- Distance
- Pickup date
- Delivery date
- Delay flag (target variable)

## 📈 Target
`delayed`: 0 = On-time, 1 = Delayed

## 🚀 Goal
Use this project to demonstrate understanding of:
- EDA and feature engineering
- Model building and evaluation
- Practical ML in logistics/supply chain domain

---

✅ Final Model & Evaluation

The final model used was a **Random Forest Classifier**, selected after hyperparameter tuning via **GridSearchCV** and evaluated using **3-fold cross-validation**.

**Final Steps Completed:**
- Label encoding of categorical hub feature  
- Split data into training and test sets (80/20)  
- Tuned `n_estimators`, `max_depth`, and `min_samples_split`  
- Exported trained model as `shipment_delay_model.pkl`

📊 **Evaluation Report:**

| Metric     | Class 0 (On-Time) | Class 1 (Delayed) |
|------------|------------------|-------------------|
| Precision  | 0.89             | 0.85              |
| Recall     | 0.93             | 0.79              |
| F1-Score   | 0.91             | 0.82              |

📌 Overall Accuracy: ~88%  
📁 [View Final Notebook](https://github.com/satyamvohra03/shipment-delay-predictor/blob/main/day9_final_model_and_evaluation.ipynb)

---


