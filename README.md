# 🏨 Hotel Booking Cancellation Prediction
<img width="1080" height="1080" alt="Blue Modern Hotel Promotion Instagram Post (2)" src="https://github.com/user-attachments/assets/6792a9e1-5dfd-4cc9-903d-780174b731b6" />

An end-to-end machine learning project that predicts whether a hotel booking will be canceled, and translates the results into concrete business actions. Includes data cleaning, EDA, feature engineering, modeling (Random Forest best), evaluation (AUC ≈ 0.97), and a presentation summarizing insights and recommendations.

## 📦 What’s in this repo
- original dataset - booking.csv
- notebooks — Jupyter notebooks (main analysis + PyCaret AutoML)
- reports — presentation slide deck

## 🎯 Objectives
- Understand booking behavior and drivers of cancellation
- Build a robust classifier to predict cancellations
- Deliver actionable recommendations for policy and ops

## 📊 Dataset (snapshot)
~36k bookings; features include adults/children counts, nights, lead time, room type, market segment type, average price, special requests, etc.; target: booking status (Canceled / Not Canceled). Key cleaning included removing invalid stays (0 week + 0 weekend nights), handling outliers, and dropping redundant columns.

## 🔍 Highlights from EDA
- **Lead time** ↑ → **cancellation likelihood** ↑; sharp rise beyond ~150 days
- **Repeat customers**: extremely reliable; **very low** cancel rate
- **Special requests**: more requests → **lower** cancellation risk
- **Market segment**: **online** drives most cancellations; **corporate/complementary** are highly reliable
- **Average price**: cancellation rate increases across price bands (instability at higher bands)

## 🤖 Modeling
- Candidates: Logistic Regression, Random Forest, Gradient Boosting, AdaBoost, SVC, KNN, Decision Tree, XGBoost; PyCaret AutoML used for comparison.
- **Best model**: Random Forest Classifier
- **ROC–AUC ≈ 0.97** (excellent separation)

## Recommendations
- See slide deck
