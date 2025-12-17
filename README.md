# 🧠 AI for Early Alzheimer’s Detection

Early detection of Alzheimer’s disease can significantly improve patient care and quality of life. This project leverages **machine learning on clinical and cognitive assessment data** to classify Alzheimer’s disease stages and support early diagnosis.

---

## 📌 Project Overview

* **Problem:** Alzheimer’s disease is often diagnosed late, reducing treatment effectiveness.
* **Solution:** Apply supervised machine learning models on structured clinical data to detect early signs of Alzheimer’s.
* **Impact:** Provides a scalable, cost-effective decision-support tool for healthcare professionals.

---

## 📊 Dataset

* **Source:** OASIS Longitudinal Alzheimer’s Dataset
* **Type:** Tabular clinical and cognitive data
* **Target Variable:** `Group`

  * Non-Demented
  * Demented
  * Converted

### Key Features

* Age
* Years of education (EDUC)
* Mini-Mental State Examination (MMSE)
* Clinical Dementia Rating (CDR)
* Estimated Total Intracranial Volume (eTIV)
* Normalized Whole Brain Volume (nWBV)
* Atlas Scaling Factor (ASF)

---

## 🧪 Methodology

1. **Data Preprocessing**

   * Removal of non-informative ID columns
   * Missing value handling using mean imputation
   * Label encoding of target classes
   * Feature scaling using standardization

2. **Models Implemented**

   * Logistic Regression (Baseline)
   * Random Forest Classifier (Primary Model)
   * Support Vector Machine (SVM)

3. **Evaluation Metrics**

   * Accuracy
   * Precision
   * Recall
   * F1-Score (weighted)
   * Confusion Matrix

4. **Robustness Check**

   * 5-fold Cross-Validation using weighted F1-score

---

## 📈 Results Summary

| Model               | Accuracy    | F1 Score | Recall   |
| ------------------- | ----------- | -------- | -------- |
| Logistic Regression | Baseline    | Moderate | Moderate |
| Random Forest       | **Best**    | **Best** | **Best** |
| SVM                 | Competitive | Good     | Good     |

* Random Forest achieved the best balance of performance metrics.
* Cognitive assessment features (MMSE, CDR) were the strongest predictors.

---

## 🔍 Explainability

* Feature importance from Random Forest was analyzed.
* Top features contribute to improved interpretability and clinical trust.

---

## ⚖️ Ethical Considerations

* This project is intended **only as a decision-support tool**.
* It does **not replace professional medical diagnosis**.
* Patient privacy and responsible AI usage are emphasized.

---

## 🚀 How to Run

1. Clone this repository

   ```bash
   git clone https://github.com/Fahad035/ai-alzheimers-detection.git
   cd ai-alzheimers-detection
   ```

2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook

   * Open the provided Jupyter / Google Colab notebook
   * Upload `oasis_longitudinal.csv`
   * Run all cells sequentially

---

## 📁 Repository Structure

```
├── notebook.ipynb        # Reproducible ML pipeline
├── README.md             # Project documentation
├── requirements.txt      # Dependencies
└── report.pdf             # Hackathon project report
```

---

## 🔮 Future Work

* Incorporate longitudinal patient history
* Combine clinical and imaging (MRI) data
* Deploy as a real-time clinical decision support system

---

## 🏁 Conclusion

This project demonstrates how machine learning can assist in **early Alzheimer’s disease detection** using accessible clinical data. With strong evaluation, interpretability, and reproducibility, it represents a practical step toward impactful healthcare AI solutions.

---

⭐ If you find this project useful, feel free to star the repository!
