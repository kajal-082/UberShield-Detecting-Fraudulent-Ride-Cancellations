# UberShield: Detecting Fraudulent Ride Cancellations

## Project Overview
UberShield is a machine learning-based project designed to detect drivers who cancel rides upon reaching the pickup location and offer offline trips at higher charges. This project is part of the Uber Tank 3.0 competition and aims to enhance ride transparency and customer trust by identifying fraudulent ride behaviors.

## Dataset
The dataset used for this project is the 'Uber Pickups in New York City' dataset. It contains ride request logs with details such as pickup location, timestamps, ride status, and other relevant features.

## Problem Statement
The objective is to analyze ride cancellation patterns and develop a model that can predict fraudulent cancellations. Fraudulent behavior includes:
- Drivers accepting rides but canceling upon reaching the pickup point.
- Drivers pushing customers towards offline rides for higher charges.
- Identifying trends based on ride timestamps, locations, and driver behaviors.

## Approach
1. **Data Preprocessing:**
   - Handling missing values.
   - Encoding categorical variables.
   - Feature engineering (creating new relevant features based on timestamps and locations).
   
2. **Model Selection:**
   - Logistic Regression, Random Forest, XGBoost, and other supervised learning techniques are tested.
   - Hyperparameter tuning to improve model performance.
   
3. **Evaluation Metrics:**
   - Precision, Recall, F1-score, and AUC-ROC to measure model effectiveness.
   
4. **Deployment (Future Scope):**
   - Implementing a real-time detection system.
   - Integrating the model with Uber’s fraud detection framework.

## Requirements
To run this project, install the following dependencies:
```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```
## Results
The best-performing model achieved [85.28]% accuracy with an F1-score of [0.85]. The results suggest that fraudulent ride cancellations can be effectively detected using machine learning techniques.

## Future Improvements
- Enhancing feature engineering with additional ride attributes.
- Integrating real-time tracking for dynamic fraud detection.
- Deploying the model using Flask or FastAPI for live predictions.
