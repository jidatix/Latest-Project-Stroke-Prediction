
# Stroke Prediction Project

## Description
This project predicts whether a person is at risk of stroke using health and demographic data. 
Features include: age, gender, hypertension, heart disease, marital status, work type, residence type, average glucose level, BMI, and smoking status.

## Key Features
- **Data Preprocessing:** Handling missing values, encoding categorical variables, scaling features, balancing dataset with SMOTE.
- **Model:** Logistic Regression (best performing), with trained model saved as `logistic_stroke_model.pkl`.
- **Evaluation:** Accuracy, Precision, Recall, F1-Score, Confusion Matrix.
- **Feature Importance:** Visualizations to understand key factors affecting stroke.
- **Deployment:** Gradio interface for real-time predictions.

## How to Use
1. Load the saved model and scaler:
```python
import joblib
model = joblib.load('logistic_stroke_model.pkl')
scaler = joblib.load('scaler.pkl')
