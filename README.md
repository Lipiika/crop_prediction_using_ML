# 🌱 Crop Prediction Using Machine Learning

This project predicts the most suitable crop to grow based on soil and environmental conditions. It uses a variety of machine learning algorithms to determine the best crop, making it useful for farmers, agricultural advisors, and agri-tech platforms.

---

## 🧠 Project Overview

Given inputs such as nitrogen (N), phosphorus (P), potassium (K), temperature, humidity, pH, and rainfall, the model suggests the ideal crop that can be cultivated in those conditions.

---

## 🧪 Dataset Features

The dataset includes the following features:

- **N**: Nitrogen level in soil  
- **P**: Phosphorus level in soil  
- **K**: Potassium level in soil  
- **Temperature**: in °C  
- **Humidity**: in %  
- **pH**: Soil pH value  
- **Rainfall**: in mm  
- **Label**: Crop name (e.g., rice, maize, mango)

Dataset Source: [Kaggle Crop Recommendation Dataset](https://www.kaggle.com/datasets)

---

## 🤖 Machine Learning Models Used

The notebook trains and compares the performance of multiple classifiers:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- K-Nearest Neighbors (KNN)  
- Support Vector Machine (SVM)  
- Naive Bayes

The dataset is scaled using `StandardScaler` to improve performance.

---

## 📊 Evaluation Metrics

For each model, performance is measured using:

- Accuracy Score  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)

At the end, the accuracy of all models is visualized using a bar chart for comparison.

---

## 💾 Model Deployment

The best-performing model can be saved using:
```python
import joblib
joblib.dump(model, 'crop_model.joblib')
