# 🧠 Parkinson's Disease Classification

This project focuses on predicting whether a person is affected by **Parkinson’s Disease** using machine learning algorithms.  
The dataset was analyzed, preprocessed, and trained using multiple classification models to compare performance and generalization.

---

## 🧰 Tools and Libraries
- **Python**
- **NumPy, Pandas** for data analysis  
- **Scikit-learn** for machine learning  
- **Matplotlib / Seaborn** for visualization  

---

## ⚙️ Models Used
Three classifiers were implemented and compared:

1. **XGBClassifier (XGBoost)**  
   - Gradient boosting algorithm providing strong predictive performance.

2. **Support Vector Machine (SVM)**  
   - Applied with RBF kernel for handling non-linear relationships in the data.

3. **RandomForestClassifier**  
   - Ensemble method combining multiple decision trees to improve accuracy and reduce overfitting.

---

## 🎯 Model Evaluation
Model performance was evaluated using:

- **Accuracy Score**
- **Classification Report (Precision, Recall, F1-Score)**
- **Confusion Matrix**

---

## 📊 Example Results

| Dataset | Metric | Score |
|----------|---------|--------|
| Training Data | Accuracy | **1.0** |
| Test Data | Accuracy | **0.872 (≈87.2%)** |

These results indicate that the model performs well on unseen data with balanced generalization between training and testing sets.

---

## 🔍 Observations
- The **training accuracy (100%)** shows perfect learning on training data.  
- The **test accuracy (87%)** suggests minor overfitting but good generalization.  
- Using **data scaling, tuning hyperparameters**, and **cross-validation** can further enhance results.

---

## 🧩 Future Improvements
- Apply **GridSearchCV** or **RandomizedSearchCV** for hyperparameter optimization.  
- Use **feature importance analysis** (from XGBoost or Random Forest) to identify the most influential attributes.  
- Integrate results into a **Streamlit dashboard** for interactive visualization and live predictions.

-
