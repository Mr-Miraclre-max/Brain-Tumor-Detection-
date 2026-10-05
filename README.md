# Brain-Tumor-Detection-
Brain Tumor Detection using MRI Images through CNN model


# 🧠 Brain Tumor Detection Using CNN

A deep learning project that uses **Convolutional Neural Networks (CNNs)** to classify brain MRI images into different tumor categories. The project covers the complete workflow from image preprocessing and model training to evaluation and prediction.

> **Disclaimer:** This project is for educational and research purposes only. It is **not a medical diagnostic tool** and should not be used to make clinical decisions.

---

## 📌 Project Overview

Brain tumors are abnormal growths of cells in the brain that can be difficult to identify manually from medical images.

In this project, a **CNN-based image classification model** is trained on brain MRI images to automatically classify images into predefined tumor categories.

The main goal is to understand how **Deep Learning and Computer Vision** can be applied to medical image classification.

---

## 🎯 Objectives

* Perform preprocessing of brain MRI images.
* Prepare the dataset for CNN training.
* Build a Convolutional Neural Network using TensorFlow/Keras.
* Train the model to classify brain MRI images.
* Evaluate model performance using appropriate metrics.
* Visualize training and validation performance.
* Test the model on new MRI images.

---

## 🗂️ Dataset

The project uses a brain MRI image dataset containing multiple classes of brain conditions.

Example classes may include:

* Glioma
* Meningioma
* Pituitary Tumor
* No Tumor

The dataset is divided into:

* **Training set** — used to train the CNN.
* **Validation set** — used to monitor model performance during training.
* **Testing set** — used to evaluate the final model.

> The exact number of images and class distribution depend on the dataset used for this project.

---

## 🛠️ Technologies Used

| Technology   | Purpose                 |
| ------------ | ----------------------- |
| Python       | Programming language    |
| TensorFlow   | Deep learning framework |
| Keras        | CNN model development   |
| NumPy        | Numerical operations    |
| Pandas       | Data handling           |
| Matplotlib   | Data visualization      |
| Google Colab | Development environment |
| GitHub       | Project version control |

---

## 🧠 Model Architecture

The CNN consists of multiple layers designed to learn visual features from MRI images.

Typical architecture:

```text
Input MRI Image
       ↓
Image Resizing & Normalization
       ↓
Convolutional Layer
       ↓
ReLU Activation
       ↓
Max Pooling
       ↓
Convolutional Layer
       ↓
ReLU Activation
       ↓
Max Pooling
       ↓
Flatten
       ↓
Dense Layer
       ↓
Dropout
       ↓
Output Layer
       ↓
Softmax Classification
```

The final output layer contains **4 neurons** when four tumor classes are used.

```python
Dense(4, activation="softmax")
```

The Softmax layer produces a probability for each class.

---

## 🔄 Project Workflow

```text
MRI Dataset
     ↓
Data Collection
     ↓
Image Preprocessing
     ↓
Image Resizing
     ↓
Normalization
     ↓
Train / Validation / Test Split
     ↓
CNN Model
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Prediction
```

---

## 📊 Model Evaluation

The model can be evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* Training vs Validation Accuracy
* Training vs Validation Loss

Example evaluation plots:

```text
Training Accuracy vs Validation Accuracy
Training Loss vs Validation Loss
```

A confusion matrix can also be used to identify which tumor classes are being confused by the model.

---

## 🔍 Prediction

After training, the model can be used to classify a new MRI image.

The prediction pipeline is:

```text
New MRI Image
      ↓
Resize Image
      ↓
Normalize Pixel Values
      ↓
CNN Model
      ↓
Class Probabilities
      ↓
Predicted Class
```

Example output:

```text
Predicted Class: Glioma
Confidence: 94.2%
```

> Confidence scores from a neural network should not be interpreted as medical certainty.

---

## 📈 Results

The final results will be added after completing model training and evaluation.

### Model Performance

| Metric              | Score |
| ------------------- | ----: |
| Training Accuracy   |     — |
| Validation Accuracy |     — |
| Test Accuracy       |     — |
| Precision           |     — |
| Recall              |     — |
| F1-Score            |     — |

---

## 📁 Project Structure

```text
Brain-Tumor-Detection/
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── notebooks/
│   └── brain_tumor_detection.ipynb
│
├── models/
│   └── brain_tumor_cnn.h5
│
├── results/
│   ├── accuracy_plot.png
│   ├── loss_plot.png
│   └── confusion_matrix.png
│
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Brain-Tumor-Detection.git
```

### 2. Open the project

The notebook can be opened using **Google Colab** or Jupyter Notebook.

### 3. Install dependencies

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn
```

### 4. Load the dataset

Place the MRI dataset in the appropriate dataset directory.

### 5. Run the notebook

Run the notebook cells sequentially to:

1. Load the dataset
2. Preprocess images
3. Create the CNN
4. Train the model
5. Evaluate the model
6. Generate predictions

---

## 🔮 Future Improvements

Possible improvements include:

* Data augmentation
* Transfer learning using ResNet, EfficientNet or MobileNet
* Hyperparameter tuning
* Cross-validation
* Improved class balancing
* Grad-CAM for model explainability
* Larger and more diverse datasets
* Deployment using Streamlit or Flask
* Web-based MRI prediction interface

---

## ⚠️ Disclaimer

This project is intended for **educational purposes only**. The model has not been validated for clinical use and should not be used to diagnose, treat, or make medical decisions regarding brain tumors.

---



---

## ⭐ Acknowledgements

Thanks to the open-source machine learning and medical imaging communities for providing datasets, frameworks, and resources that helped in developing this project.

If you found this project useful, consider ⭐ starring the repository.
