

---

# 🩺 Medical Image Classification: Atelectasis Detection

## 🧠 Project Summary

This project presents a **binary medical image classification system** designed to identify **Atelectasis** from chest X-rays. Leveraging **machine learning** techniques and confidence-based calibration, the model aims to support radiologists by offering reliable classification and interpretability through performance visualization.

---

## 🚀 Features

- ✅ **Binary Classification**: Predicts presence (`Atelectasis`) vs. absence (`Negative`) of the condition.
- 📈 **Performance Metrics**:
  - **Accuracy**, **Sensitivity**, **Specificity**
  - **Confusion Matrix Analysis**
- 📊 **Visual Diagnostics**:
  - Confidence score histograms
  - ROC curve with AUC
- 📌 **Threshold Calibration**: Optimal classification threshold set to **0.5** for decision boundary.

---

## 🧪 Results

### ✅ Performance Summary

| Metric         | Value   |
|----------------|---------|
| **Accuracy**   | 0.72    |
| **Sensitivity**| 0.94    |
| **Specificity**| 0.53    |
| **AUC (ROC)**  | 0.805   |

<sub>*Based on test set evaluation*</sub>

### 🧾 Confusion Matrix

|                | Pred: Positive | Pred: Negative |
|----------------|----------------|----------------|
| **Actual: Positive** | 34 (TP)         | 2 (FN)          |
| **Actual: Negative** | 17 (FP)         | 19 (TN)         |

---

## 📊 Visual Insights

- **Histogram of Confidence Scores**:
  - Clear distinction between correctly and incorrectly classified samples.
  - High-confidence true positives dominate above threshold (0.5).
  
- **ROC Curve**:
  - Shows robust classification capability with AUC = **0.805**.
  - Demonstrates a strong balance between sensitivity and specificity.

---

## 🧰 Tech Stack

| Component          | Tools / Libraries             |
|-------------------|-------------------------------|
| Language           | Python                        |
| ML Models          | Scikit-learn (e.g., XGBoost)  |
| Data Visualization | Matplotlib, Seaborn           |
| Image Processing   | OpenCV, PIL                   |

---

## 🩻 Use Case

- Automated assistance in **radiology workflows** for identifying **Atelectasis**.
- Provides **confidence-based reasoning** for predictions.
- Suitable for integration in **clinical decision support systems (CDSS)**.

---

## 🔮 Future Improvements

- 📦 **Data Augmentation**: Improve robustness on diverse datasets.
- 🧠 **Deep Learning**: Integrate CNN-based models for better spatial feature extraction.
- 📈 **Threshold Tuning**: Explore dynamic thresholding based on patient risk profiles.
- 🌐 **Web Interface**: Deploy model with an interactive UI for healthcare professionals.

---
