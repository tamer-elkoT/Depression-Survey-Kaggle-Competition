🌟 Depression Detection from Survey Data — Advanced Machine Learning Project
🎯 Achieved 92.09% Accuracy | 🏆 Kaggle Top 8 Ranking | 👨‍💻 Freelancer: Tamer Elkot
<p align="center"> <img src="images/cover.jpg" width="80%"> </p>
🚀 Project Overview

This project focuses on predicting depression from large-scale survey data using advanced machine learning techniques.
With more than 165,000 records and 20+ psychological, demographic, and lifestyle features, the goal was to identify individuals at high risk of depression.

The final model achieved:

Metric	Score
Accuracy	92.09%
AUC-ROC	0.941
Precision	89.5%
Recall	87.2%
Leaderboard Rank	Top 8 on Kaggle
📌 Table of Contents

Project Motivation

Dataset Overview

Project Pipeline

Data Preprocessing

EDA Highlights

Feature Engineering

Modeling & Optimization

Results & Insights

Business Impact

How to Run the Project

Future Work

Credits

🎯 Project Motivation

Depression is a global mental health challenge, yet early detection remains difficult.
This project aims to:

Detect potential depression early

Support healthcare and student wellness systems

Understand hidden risk patterns in demographics, lifestyle, and psychological factors

Build a scalable model for large populations

🧠 Dataset Overview

Records: 165,000+ participants

Target: Depression (Yes/No)

Features include:

Age

Gender

Region & City

Sleep duration

Dietary habits

Academic pressure

Work pressure

Study satisfaction

Job satisfaction

Profession & salary rank

CGPA (for students)

🛠️ Project Pipeline
Data Cleaning → Preprocessing → EDA → Feature Engineering →
Balancing → Model Training → Hyperparameter Tuning → Ensemble →
Evaluation → Insights & Reporting

🔧 Data Preprocessing
✔ Domain-based imputation
Feature	Strategy
Academic Pressure	Set to 0 for working professionals
Work Pressure	Set to 0 for students
CGPA	Assigned 0 for non-students
✔ Handling missing & inconsistent values

Standardized categorical values and grouped rare professions.

✔ Encoding

One-hot encoding for regions & cities

Ordinal encoding for sleep quality, dietary habits

Binary flag for student status

📊 EDA Highlights
🔹 Depression by Age Group

Age 18–25 had the highest depression rates.

<p align="center"> <img src="images/age_group_depression.png" width="65%"> </p>
🔹 Depression by Gender

Males showed a slightly higher depression rate — likely due to sample distribution.

<p align="center"> <img src="images/gender_depression.png" width="65%"> </p>
🔹 Sleep Duration Impact

Less than 5 hours of sleep drastically increases depression probability.

<p align="center"> <img src="images/sleep_duration.png" width="65%"> </p>
🔹 Region & City

South India had the highest depression prevalence.

<p align="center"> <img src="images/region_city.png" width="70%"> </p>
🧩 Feature Engineering

Age binning into logical groups

Profession mapped to salary ranks

Behavioral segmentation (Student vs Professional)

Geographic encoding

Sleep/Diet ordinal scoring

SMOTE-ENN for class balancing

🤖 Modeling & Optimization

Models Tested:

Logistic Regression

Random Forest

XGBoost

Neural Network

Ensemble (XGBoost + Logistic Regression)

Best Model:

⭐ XGBoost + Ensemble

RandomizedSearchCV

Optuna optimization

Stratified K-Fold validation

🏆 Final Results
✔ Best Model Accuracy: 92.09%
✔ AUC-ROC: 0.941
✔ Top 8 on Kaggle Leaderboard
Model	Score
XGBoost Ensemble	92.09%
Random Forest	88.4%
Logistic Regression	84.7%
Neural Network	87.9%
💡 Key Insights

18–25 age group is most vulnerable

<5 hours sleep increases depression risk by ~67%

Students have 28% higher rates than working professionals

South India shows 23% higher prevalence

Low-income professions correlate with higher depression levels

🏢 Business & Health Impact
✔ Early Detection

Accurate prediction enables faster mental health intervention.

✔ Scalable

Model handles over 165K+ records smoothly.

✔ ROI Potential

Preventive screening reduces long-term healthcare cost.

✔ Real-World Application

Hospitals

Universities

Corporate wellness programs

Telemedicine platforms

🖥️ How to Run the Project
# Clone the repository
git clone https://github.com/<your-username>/Depression-Detection-From-Survey-Data.git

cd Depression-Detection-From-Survey-Data

pip install -r requirements.txt

# Run the notebook
jupyter notebook

🚀 Future Enhancements

Deep Learning models (LSTMs, TabNet)

Real-time depression monitoring API

Explainable AI (SHAP, LIME)

Integration with mobile health apps

Personalized recommendations system

👤 Credits

Freelancer / Developer:

Eng. Tamer Elkot

Advanced ML Engineer | AI Engineer
Top 8 Kaggle Competition — Depression Prediction
