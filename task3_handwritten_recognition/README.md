# ✍️ Task 3 – Handwritten Character Recognition
### CodeAlpha Machine Learning Internship

---

## 📌 Objective
Identify handwritten **digits and alphabets** using **image processing** and **deep learning** with a Convolutional Neural Network (CNN).

---

## 📂 Project Structure
```
task3_handwritten_recognition/
│
├── handwritten_recognition.ipynb   # Main Jupyter Notebook
└── README.md
```

---

## 📊 Dataset
- **Name:** MNIST — Modified National Institute of Standards and Technology
- **Source:** Built into `tensorflow.keras.datasets` (auto-downloaded)
- **Size:** 70,000 grayscale images (60,000 train + 10,000 test)
- **Image Size:** 28 × 28 pixels
- **Classes:** 10 digits (0–9)

---

## 🧠 Model Architecture — CNN

```
Input (28×28×1)
    ↓
Conv2D(32) → BatchNorm → Conv2D(32) → MaxPool → Dropout(0.25)
    ↓
Conv2D(64) → BatchNorm → Conv2D(64) → MaxPool → Dropout(0.25)
    ↓
Flatten → Dense(256) → BatchNorm → Dropout(0.5)
    ↓
Dense(10, softmax)  →  Output
```

---

## ⚙️ Key Features

| Feature | Detail |
|---------|--------|
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Batch Size | 128 |
| Max Epochs | 20 (with Early Stopping) |
| Callbacks | EarlyStopping, ReduceLROnPlateau |
| Regularization | BatchNormalization + Dropout |

---

## 📈 Results

| Metric | Value |
|--------|-------|
| Test Accuracy | ~99% |
| Test Loss | ~0.03 |

### Visualisations Generated
- Sample digit grid (3 × 10)
- Training accuracy & loss curves
- Confusion matrix (10 × 10)
- Predictions vs actual (Green = correct, Red = wrong)

---

## ▶️ How to Run

### Option 1 — Google Colab (Recommended)
1. Upload `handwritten_recognition.ipynb` to [colab.research.google.com](https://colab.research.google.com)
2. Click **Runtime → Run all**
3. Dataset downloads automatically ✅

### Option 2 — Local Jupyter
```bash
pip install tensorflow matplotlib seaborn numpy scikit-learn
jupyter notebook handwritten_recognition.ipynb
```

---

## 🛠️ Tech Stack
- Python 3.x
- TensorFlow / Keras
- NumPy, Matplotlib, Seaborn
- Scikit-learn (metrics)

---

## 👤 Author
**CodeAlpha Internship – June Batch**
Task 3 of 4 | Machine Learning Track
