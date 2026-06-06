# 🏛️ Landmark Detection Using Deep Learning

## 📌 Overview

This project implements a **Landmark Detection and Classification System** using Deep Learning techniques. The model is trained on landmark images and predicts the corresponding landmark class from a given image.

The project utilizes the **VGG19 Convolutional Neural Network (CNN)** architecture with TensorFlow/Keras for feature extraction and landmark classification.

---

## 🚀 Features

* Image preprocessing and dataset analysis
* Landmark label encoding and decoding
* Data visualization and exploration
* Deep learning-based image classification
* VGG19 transfer learning architecture
* Batch training and validation
* Landmark prediction from images
* Performance evaluation on validation data

---

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* OpenCV
* Matplotlib
* PIL (Python Imaging Library)
* Scikit-Learn

---

## 📊 Dataset

The project uses a landmark image dataset containing:

* Image IDs
* Landmark IDs (Labels)
* Landmark images stored in nested folders

Example:

| Image ID | Landmark ID |
| -------- | ----------- |
| abc123   | 1001        |
| xyz456   | 2045        |

The dataset is filtered and processed before training.

---

## 🔍 Data Analysis

The notebook performs:

* Dataset loading
* Landmark frequency analysis
* Distribution visualization
* Class count statistics
* Sample image visualization

### Example Analysis

* Number of landmark classes
* Number of training samples
* Landmark frequency histogram
* Dataset imbalance analysis

---

## 🧠 Model Architecture

The model is built using **VGG19** as the base network.

### Architecture

```
Input Image
      ↓
VGG19 Convolutional Layers
      ↓
Batch Normalization
      ↓
Dropout
      ↓
Dense Layer
      ↓
Softmax Output Layer
```

### Hyperparameters

| Parameter     | Value                           |
| ------------- | ------------------------------- |
| Learning Rate | 0.0001                          |
| Optimizer     | RMSprop                         |
| Loss Function | Sparse Categorical Crossentropy |
| Batch Size    | 64                              |
| Epochs        | 1 (can be increased)            |

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/landmark-detection.git

cd landmark-detection
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install tensorflow keras numpy pandas matplotlib pillow opencv-python scikit-learn
```

---

## ▶️ Running the Project

### Open Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
LANDMARK_DETECTION_PROJECT.ipynb
```

Run all cells sequentially.

---

## 📈 Training

The model is trained using mini-batch gradient descent.

```python
model.fit(
    X_train,
    y_train
)
```

Training includes:

* Dataset shuffling
* Batch generation
* Label encoding
* Validation evaluation

---

## 🎯 Prediction

The trained model predicts the landmark category of an input image.

```python
result = model.predict(image)
predicted_class = np.argmax(result)
```

The predicted label can then be converted back to the original landmark ID.

---

## 📉 Evaluation

The notebook evaluates:

* Prediction accuracy
* Validation performance
* Correct and incorrect classifications

Metrics used:

* Accuracy
* Classification comparison

---

## 🔮 Future Improvements

* Increase training epochs
* Use pretrained ImageNet weights
* Implement data augmentation
* Fine-tune deeper layers
* Deploy as a web application
* Add real-time landmark recognition
* Improve model accuracy using EfficientNet or Vision Transformers

---

## 📚 Learning Outcomes

Through this project, the following concepts are explored:

* Computer Vision
* Convolutional Neural Networks
* Transfer Learning
* Image Classification
* Data Preprocessing
* Model Evaluation
* Deep Learning with TensorFlow

---
