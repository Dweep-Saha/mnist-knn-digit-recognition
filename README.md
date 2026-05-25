# MNIST Digit Recognition — KNN & CNN

Classifies handwritten digits (0–9) from the MNIST dataset using two ML approaches:
- **K-Nearest Neighbors (KNN)**
- **Convolutional Neural Network (CNN)**

---

## Notebooks

- [`Digits_recognition_KNN.ipynb`](Digits_recognition_KNN.ipynb) — Baseline (scikit-learn KNN)
- [`Digits_recognition_CNN.ipynb`](Digits_recognition_CNN.ipynb) — Deep Learning (TensorFlow/Keras CNN)

---

## Tech Stack

- Python, NumPy, Matplotlib / Seaborn
- Keras (TensorFlow backend) — for MNIST loading & CNN
- scikit-learn — for KNN

---

## Approach

### KNN:
1. Load MNIST dataset (28×28 grayscale images)
2. Normalize pixel values (0–1)
3. Flatten images (28×28 → 784 features)
4. Train/test using KNeighborsClassifier
5. Evaluate accuracy, confusion matrix

### CNN:
1. Load & preprocess MNIST (reshape & scale to [28,28,1])
2. (Optional) Data augmentation (rotation, shift, zoom)
3. Build & train a simple CNN (Conv2D → MaxPool → Dense → Dropout)
4. Evaluate accuracy, confusion matrix, learning curves

---

## Results

| Model | Test Accuracy | Framework             |
|-------|---------------|-----------------------|
| **KNN** | 97.05%       | scikit-learn          |
| **CNN** | 99.30%       | TensorFlow (Keras)    |

---

## How to Run

1. Open **Digits_recognition_KNN.ipynb** or **Digits_recognition_CNN.ipynb**  
   in **Google Colab** or **Jupyter Notebook**
2. Run all cells step by step  
   (Install required packages if necessary or use `requirements.txt`)

---

## Credits

- [MNIST Dataset – Yann LeCun](http://yann.lecun.com/exdb/mnist/)
