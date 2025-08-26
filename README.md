# Titanic Data Insights 🚢

## 📌 Project Overview
This project analyzes the famous Titanic dataset to predict passenger survival using Machine Learning.  
The notebook focuses on model training, hyperparameter tuning, evaluation, and saving the final model.  

You can view and run the notebook directly on Google Colab here:  
👉 [Open in Colab](https://colab.research.google.com/drive/1vn9v-fl44y4YQ93OZ_GKUmGUnoOI-Kkk?usp=sharing)

---

## 🔎 Notebook Highlights
The notebook includes the following steps:

1. **Dropping Unnecessary Columns**  
   - Removed irrelevant data before training.  

2. **Model Training**  
   - Logistic Regression  
   - Decision Tree  
   - Random Forest  

3. **Hyperparameter Tuning**  
   - Applied tuning for all three models.  

4. **Evaluation**  
   - Classification Report (Precision, Recall, F1-score)  
   - Confusion Matrix (visualized)  
   - ROC Curve & AUC  

5. **Final Model Selection**  
   - Logistic Regression chosen as the best model.  
   - Model saved using `joblib` in `.pkl` format.  

---

## 📊 Results
- **Best Model:** Logistic Regression  
- **Performance Metrics:** Balanced precision, recall, and F1-score  
- **Model File:** `logistic_regression_model.pkl`  

---

## 💾 How to Use the Saved Model
```python
import joblib

# Load the saved model
model = joblib.load("logistic_regression_model.pkl")

# Predict on new data
y_pred = model.predict(X_new)
