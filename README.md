# 🫘 Dry Bean Classification using SVM, PCA, and GridSearchCV

This project focuses on classifying seven types of dry beans using morphological features and Support Vector Machine (SVM). The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/dry+bean+dataset).

📅 **Date Completed**: June 2, 2025  
🎓 **Context**: Machine Learning course assignment (multi-class classification)  

---

## 📌 Objectives

- Understand the structure of the Dry Bean dataset
- Perform EDA (Exploratory Data Analysis)
- Build a baseline SVM model
- Apply PCA to reduce dimensionality
- Tune SVM hyperparameters with GridSearchCV
- Evaluate and compare model performance

---

## 🛠️ Tools & Libraries

- **Google Colab** (Python)
- Python: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

---

## 📊 Dataset Description

- **Source**: UCI Machine Learning Repository  
- **Link**: [Dry Bean Dataset](https://archive.ics.uci.edu/ml/datasets/dry+bean+dataset)
- **Samples**: 13,611
- **Features**: 16 numerical
- **Target classes**:  
  `Barbunya`, `Bombay`, `Cali`, `Dermason`, `Horoz`, `Seker`, `Sira`

---

## 🧪 Experiments and Results

| Model                  | PCA Applied | Tuning | CV Accuracy | Test Accuracy | Notes |
|-----------------------|-------------|--------|--------------|----------------|-------|
| Baseline SVM          | ❌ No        | ❌ No   | 93.13%       | 92.00%         | Strong initial performance |
| PCA + SVM             | ✅ Yes       | ❌ No   | 89.36%       | 90.00%         | Lower dimension, slightly lower accuracy |
| Tuned SVM (GridSearch)| ❌ No        | ✅ Yes  | 93.31%       | 92.00%         | Best macro F1-score |

📌 **Best model**: SVM with `C=10`, `kernel='rbf'`, `gamma='scale'`

---

## 🧾 Key Takeaways

- SVM performs very well on multi-class classification with proper preprocessing.
- PCA can reduce model complexity with acceptable trade-offs in accuracy.
- GridSearchCV improves performance and class balance significantly.

---
## 🔗 Reference

- Dataset: [UCI Dry Bean Dataset](https://archive.ics.uci.edu/ml/datasets/dry+bean+dataset)
