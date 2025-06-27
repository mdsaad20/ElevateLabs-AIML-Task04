# 🧠 Logistic Regression Binary Classifier

This project demonstrates a complete machine learning pipeline for binary classification using **Logistic Regression** on the **Breast Cancer Wisconsin Diagnostic Dataset**. The objective is to classify tumors as malignant or benign based on various features computed from digitized images of fine needle aspirates (FNA) of breast masses.

---

## 📁 Dataset

- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- Records: 569
- Features: 30 numerical input features
- Target: 
  - `M`: Malignant (1)
  - `B`: Benign (0)

---

## ⚙️ Tools Used

- **Python**
- **Scikit-learn**
- **Pandas**
- **Matplotlib**
- **Seaborn**

---

## 🚀 Project Steps

1. **Load & Clean Data**  
   - Removed unnecessary columns (`id`, `Unnamed: 32`)  
   - Converted `diagnosis` to binary format (M = 1, B = 0)

2. **Preprocessing**  
   - Train-test split (80-20)  
   - Standardized features using `StandardScaler`

3. **Modeling**  
   - Trained a Logistic Regression model  
   - Used `predict_proba()` for ROC-AUC analysis

4. **Evaluation Metrics**
   - **Confusion Matrix**
   - **Classification Report** (Precision, Recall, F1-Score)
   - **ROC Curve & AUC Score**

---

## 📊 Results

- **Accuracy**: ~96%
- **Precision (Malignant)**: 97%
- **Recall (Malignant)**: 93%
- **ROC AUC Score**: 0.996 (Excellent)

---

## 📈 Visuals

- Confusion matrix heatmap
- ROC Curve with AUC

---

## 🧮 Logistic Regression & Sigmoid

The logistic regression model uses the **sigmoid function** to convert a linear combination of inputs into a probability. This probability is compared against a threshold (default: 0.5) to decide class membership.

---

## 📂 How to Run

1. Clone the repository or copy the `.py`/`.ipynb` file.
2. Install dependencies:
   ```
   pip install pandas scikit-learn matplotlib seaborn
   ```
3. Run the script or notebook.