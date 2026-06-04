# 👕 Fashion-MNIST Classification using Deep Learning

## 📌 Overview

This project implements and compares multiple Deep Learning models for image classification using the Fashion-MNIST dataset. The goal is to classify grayscale images of clothing items into one of ten fashion categories and evaluate the performance of different neural network architectures.

The project explores:

* Artificial Neural Network (ANN)
* Basic Convolutional Neural Network (CNN)
* Deeper CNN with Batch Normalization and Dropout

A detailed comparison of model performance is conducted using accuracy, loss, classification reports, confusion matrices, and prediction analysis.

---

## 🎯 Project Objectives

* Preprocess and prepare image data for deep learning.
* Build and compare ANN and CNN architectures.
* Evaluate model performance on unseen test data.
* Analyze strengths and weaknesses of each model.
* Understand the impact of convolutional layers on image classification tasks.

---

## 📂 Dataset

The project uses the **Fashion-MNIST** dataset provided by Keras.

### Dataset Details

* 60,000 Training Images
* 10,000 Test Images
* Image Size: 28 × 28 pixels
* Grayscale Images
* 10 Fashion Categories

| Label | Category    |
| ----- | ----------- |
| 0     | T-Shirt/Top |
| 1     | Trouser     |
| 2     | Pullover    |
| 3     | Dress       |
| 4     | Coat        |
| 5     | Sandal      |
| 6     | Shirt       |
| 7     | Sneaker     |
| 8     | Bag         |
| 9     | Ankle Boot  |

---

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib
* Plotly
* Scikit-learn
* Jupyter Notebook

---

## 🔄 Project Workflow

### 1. Data Preparation

* Load Fashion-MNIST dataset
* Normalize pixel values (0–255 → 0–1)
* Reshape images to (28, 28, 1)
* One-hot encode labels

### 2. Model Development

#### ANN Model

Architecture:

* Flatten Layer
* Dense (128, ReLU)
* Dense (64, ReLU)
* Dense (10, Softmax)

#### Basic CNN Model

Architecture:

* Conv2D (32 filters)
* MaxPooling2D
* Conv2D (64 filters)
* MaxPooling2D
* Flatten
* Dense Layer
* Output Layer

#### Deeper CNN Model

Architecture:

* Conv2D Layers
* Batch Normalization
* MaxPooling Layers
* Dropout Layers
* Dense Layers
* Softmax Output Layer

---

## 🚀 Training Strategy

To improve model performance and prevent overfitting:

### Early Stopping

* Monitors validation loss
* Stops training when performance stops improving
* Restores best model weights

### Model Checkpointing

* Saves best model weights during training
* Enables evaluation using best-performing model

---

## 📊 Model Evaluation

The following evaluation techniques were used:

* Test Accuracy
* Test Loss
* Classification Report
* Confusion Matrix
* Training Accuracy Curves
* Validation Accuracy Curves
* Training Loss Curves
* Validation Loss Curves

---

## 📈 Results & Findings

### Key Observations

✅ CNN models significantly outperformed the ANN model.

✅ Convolutional layers effectively captured spatial features from images.

✅ The Basic CNN achieved the best balance between performance and complexity.

✅ The Deeper CNN introduced more complexity but did not consistently outperform the Basic CNN.

### Conclusion

The **Basic CNN model** delivered the strongest overall performance for Fashion-MNIST classification. The results clearly demonstrate the advantage of Convolutional Neural Networks over traditional Artificial Neural Networks for image classification tasks.

---

## 🔍 Prediction Analysis

The project includes:

* Visualization of correctly classified images
* Visualization of misclassified images
* Prediction confidence analysis
* Model behavior inspection

These analyses help understand where the model performs well and where improvements can be made.

---

## 📁 Project Structure

```text
Fashion-MNIST Classification/
│
├── Fashion-MNIST Classification.ipynb
├── best_ann_model_weights.weights.h5
├── best_basic_cnn_model_weights.weights.h5
├── best_deeper_cnn_model_weights.weights.h5
└── README.md
```

---

## ▶️ How to Run

### Clone the Repository

```bash
git clone https://github.com/SakshiSrivastav94/AI_Projects.git
```

### Navigate to the Project Folder

```bash
cd Fashion-MNIST\ Classification
```

### Install Dependencies

```bash
pip install tensorflow numpy pandas matplotlib plotly scikit-learn
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open **Fashion-MNIST Classification.ipynb** and run all cells sequentially.

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Deep Learning Fundamentals
* Artificial Neural Networks (ANN)
* Convolutional Neural Networks (CNN)
* Image Classification
* TensorFlow & Keras
* Model Evaluation Techniques
* Computer Vision Workflows

---

## 🔮 Future Improvements

* Hyperparameter Optimization
* Data Augmentation
* Transfer Learning
* Advanced CNN Architectures
* Model Deployment using Streamlit or Flask

---

## 👩‍💻 Author

**Sakshi Srivastav**

Aspiring Data Scientist | Machine Learning Enthusiast | Deep Learning Practitioner

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

