# Car Resale Price Prediction Model

This project presents a comparative study of machine learning models to predict automobile resale prices using real-world data. We implemented and evaluated **Decision Tree**, **Random Forest**, and **Artificial Neural Networks (ANN)** to estimate car resale prices based on vehicle features such as mileage, transmission, fuel type, age, and more.

## Project Overview

- **Timeline:** Oct 2024 – Dec 2024  
- **Goal:** Predict used car resale prices accurately using ML models  
- **Best Performing Model:** Random Forest (MSE: 138M, RMSE: 368K, R²: 0.89)  
- **Tools & Libraries:** Python, Pandas, NumPy, Scikit-learn, TensorFlow/Keras, Matplotlib, Seaborn

---

## Dataset

The dataset included:
- Car model, year of registration
- Mileage, fuel type, transmission type
- Insurance details, owner type, location, distance driven

### Preprocessing steps:
- Missing value treatment
- One-hot encoding for categorical variables
- Normalization of numeric features
- 80/20 Train-Test Split

---

## Models Implemented

### 1. **Decision Tree Regressor**
- Intuitive and interpretable
- Tuned with `max_depth = 9`
- Accuracy: 85% (Test), RMSE: 431K

### 2. **Random Forest Regressor**
- Ensemble model for high performance
- Hyperparameter tuning via GridSearchCV
- **Best results:** MSE: 138M, RMSE: 368K, R²: 0.89

### 3. **Artificial Neural Network (ANN)**
- Built with Keras Sequential model
- Architecture: 4 hidden layers (64 → 32 → 16 → 8 neurons)
- Accuracy: 83%, RMSE: 448K
- Higher training complexity, lower interpretability

---

## Performance Comparison

| Model          | Accuracy | MSE            | RMSE     | R² Score |
|----------------|----------|----------------|----------|----------|
| Decision Tree  | 85%      | 186B           | 431K     | 0.82     |
| Random Forest  | 77.5%    | **138B**       | **368K** | **0.89** |
| ANN            | 83%      | 201B           | 448K     | 0.79     |

---

## Key Insights

- **Top predictive features:** Mileage, Transmission, Year of Registration
- **Best trade-off:** Random Forest offered the best accuracy + generalization
- **Most interpretable model:** Decision Tree
- ANN captured non-linear patterns but at the cost of interpretability

---

## References
Selvakanmani et al., "Automated Prediction for Car Resale Values Using AI", ICACCS, 2024

Lavanya et al., "Vehicle Resale Price Prediction using Machine Learning", Juni Khyat, 2021

Dholiya et al., "Automobile Resale System Using Machine Learning", IRJET, 2019
