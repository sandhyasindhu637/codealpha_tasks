# Task 4 – Disease Prediction from Medical Data
### CodeAlpha Machine Learning Internship

---

## 📌 Objective
Predict the **possibility of diabetes** in patients based on medical features using supervised classification algorithms.

---

## 📂 Project Structure
```
Task4_Disease_Prediction/
│
├── disease_prediction.py          # Main Python script
├── disease_prediction.ipynb       # Jupyter Notebook (detailed walkthrough)
├── disease_prediction_results.png # Output visualizations
└── README.md
```

---

## 📊 Dataset
- **Name:** Pima Indians Diabetes Dataset  
- **Source:** [UCI ML Repository](https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv)  
- **Size:** 768 samples × 9 features  
- **Target:** `Outcome` — 0 (No Diabetes), 1 (Diabetes)

### Features
| Feature | Description |
|---------|-------------|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body mass index |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age in years |
| **Outcome** | **Target: 1 = Diabetic, 0 = Not Diabetic** |

---

## 🤖 Models Used
| Model | Description |
|-------|-------------|
| Logistic Regression | Baseline linear classifier |
| Random Forest | Ensemble of decision trees |
| SVM (RBF Kernel) | Support Vector Machine |
| XGBoost | Gradient boosting (if installed) |

---

## 📈 Results

Models are evaluated on:
- **Test Accuracy**
- **5-Fold Cross-Validation Accuracy**
- **Classification Report** (Precision, Recall, F1-Score)

Visualizations include:
- Model accuracy comparison bar chart
- Confusion matrix for best model
- Feature importance (Random Forest)
- Glucose vs BMI scatter plot

---

## ▶️ How to Run

### 1. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

### 2. Run the script
```bash
python disease_prediction.py
```

### 3. Or open the Notebook
```bash
jupyter notebook disease_prediction.ipynb
```

---

## 🛠️ Tech Stack
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

## 👤 Author
**CodeAlpha Internship – June Batch**  
Task 4 of 4 | Machine Learning Track
