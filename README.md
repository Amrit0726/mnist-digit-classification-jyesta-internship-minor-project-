# Handwritten Digit Classification — MNIST

A beginner-friendly machine learning project that classifies handwritten digits (0–9) using the MNIST dataset. Built as part of the **Jyesta Internship Training Program**.

---

##  Project Overview

The goal is to train models that can accurately identify handwritten digits from 28×28 grayscale images. Multiple classification approaches are compared to understand how different algorithms perform on image data.

---

##  Dataset

- **MNIST** — 60,000 training images + 10,000 test images
- Each image is 28×28 pixels, grayscale
- 10 classes (digits 0 through 9)
- Loaded directly via `tensorflow.keras.datasets.mnist`

---

##  Models Implemented

| Model | Accuracy (approx.) |
|---|---|
| Logistic Regression | ~91% |
| SVM (RBF Kernel) | ~96% |
| MLP Neural Network | ~98% |
| CNN | ~99.2% |
| CNN + Data Augmentation | ~99.3% |

> Models were trained on varying subsets. Classical ML models (LR, SVM) used 10k samples for speed; neural networks used the full 60k training set.

---

##  Tech Stack

- Python 3.10
- TensorFlow / Keras
- Scikit-learn
- NumPy, Pandas
- Matplotlib, Seaborn

---

##  How to Run

**1. Clone the repo**
```bash
git clone https://github.com/<your-username>/mnist-digit-classification.git
cd mnist-digit-classification
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Open the notebook**
```bash
jupyter notebook MNIST_Digit_Classification.ipynb
```
Or open directly in [Google Colab](https://colab.research.google.com/) by uploading the `.ipynb` file.

---

##  Notebook Structure

```
1. Data Loading & Exploration
2. Data Preprocessing (normalisation, reshaping)
3. Model Training (LR → SVM → MLP → CNN)
4. Model Evaluation (accuracy, precision, recall, F1, confusion matrix)
5. Hyperparameter Tuning
6. Extension — CNN with Data Augmentation
7. Misclassified digit visualisation
```

---

##  Sample Results

- CNN achieves **~99.2% test accuracy** on 10,000 unseen images
- Most common misclassifications occur between visually similar digits: `4↔9`, `3↔8`, `7↔1`

---

##  Author

**Amrit Noor Singh**  
B.Tech  (Data Science) — NIT Jalandhar, Batch of 2028  
