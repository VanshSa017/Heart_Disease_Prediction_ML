# 📊 Heart Disease Prediction Using Machine Learning

## 🔍 Project Overview

This project focuses on building and evaluating multiple **classification models** on a structured dataset using a complete **end-to-end machine learning pipeline**. The objective was to achieve **strong generalization performance** while maintaining model interpretability and robustness.

Several classical and advanced machine learning algorithms were implemented, evaluated, and compared. Although **ensemble techniques were explored**, they were **not included in the final solution** due to degraded validation performance.

---

## 🧠 Models Implemented

The following classification algorithms were trained and evaluated:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* AdaBoost Classifier
* XGBoost Classifier
* CatBoost Classifier
* LightGBM Classifier

Each model was tuned with reasonable hyperparameters and evaluated using consistent metrics.

---

## ⚙️ Preprocessing Pipeline

The dataset underwent the following preprocessing steps:

1. Handling missing values
2. Encoding categorical variables
3. Feature scaling using **StandardScaler** (for numerical features)
4. Train-test split with index alignment preserved

All preprocessing steps were applied **only on training data** and then transformed on test data to avoid data leakage.

---

## 📈 Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

The final model was selected based on **overall generalization performance**, not just training accuracy. **Random Forest** gave the best performace.

---

## 🏆 Final Model Selection

After comparative evaluation, the best-performing model was selected based on:

* Strong validation/test metrics
* Stable performance across folds
* Lower overfitting tendency
* Interpretability 

---

## 🧪 Reproducibility

To ensure reproducibility:

* Random seeds (`random_state`) were fixed
* Consistent preprocessing and evaluation strategy was followed

---

## 📂 Project Structure (High-Level)

```
├── datasets/
│   ├── dataset_raw.csv
│   └── test_data.csv
|   └── train_data.csv
├── notebooks/
│   ├── model_training.ipynb
│   └── preprocessing.ipynb
├── models/
│   ├── RandomForest.pkl
|   └── scaling_model.pkl
├── README.md
└── requirements.txt
```

---

## 🚀 Key Takeaways

* Ensembling is **not always beneficial**; empirical evaluation matters
* Simpler models can outperform complex pipelines when well-tuned
* Proper preprocessing and validation are critical for real-world performance

---

## 📌 Future Improvements

* Advanced hyperparameter optimization (Bayesian Search)
* Feature engineering based on domain knowledge
* Cross-validation-based model selection

---

## 📌 How to Run the Project

1. Clone the repository
```bash
git clone  https://github.com/VanshSa017/Heart_Disease_Prediction_ML.git
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Run the notebook or script
```bash
python preprocessing.ipynb
python model_training.ipynb 
```

---

## ✨ Author Note

This project was built with a **practical, performance-first mindset**, prioritizing real-world generalization over theoretical complexity.
