# ❤️ Heart Disease Predictor

## 📌 Project Overview

Heart Disease Predictor is a Machine Learning classification project that predicts whether a patient is likely to have heart disease based on various medical attributes.

The project demonstrates a complete end-to-end Machine Learning workflow, including:

* Data Collection
* Exploratory Data Analysis (EDA)
* Data Preprocessing
* Feature Engineering
* Model Training
* Model Evaluation
* Feature Importance Analysis

Multiple classification algorithms are trained and compared to identify the most effective model for heart disease prediction.

---

## 🎯 Project Objective

The primary objective of this project is to build an accurate classification model that can predict the presence of heart disease using patient medical data.

The project also aims to:

* Understand the factors contributing to heart disease.
* Compare different classification algorithms.
* Evaluate model performance using multiple metrics.
* Identify the most influential medical features.

---

## 📂 Dataset Information

The dataset used in this project is the **Heart Disease UCI Dataset** obtained through Kaggle.

### Features Included

| Feature  | Description                       |
| -------- | --------------------------------- |
| age      | Age of patient                    |
| sex      | Gender                            |
| cp       | Chest pain type                   |
| trestbps | Resting blood pressure            |
| chol     | Cholesterol level                 |
| fbs      | Fasting blood sugar               |
| restecg  | Resting ECG results               |
| thalach  | Maximum heart rate achieved       |
| exang    | Exercise-induced angina           |
| oldpeak  | ST depression induced by exercise |
| slope    | Slope of peak exercise ST segment |
| ca       | Number of major vessels           |
| thal     | Thalassemia type                  |
| num      | Heart disease target variable     |

### Target Variable

* **0** → No Heart Disease
* **1** → Heart Disease Present

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Data Analysis

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-Learn

### Dataset Source

* KaggleHub API

---

## 📊 Exploratory Data Analysis (EDA)

The project begins with a comprehensive analysis of the dataset.

### Data Inspection

* Dataset shape analysis
* Feature type identification
* Missing value detection
* Statistical summary generation

### Target Variable Analysis

The distribution of patients with and without heart disease is visualized to understand class balance.

### Feature Analysis

Relationships between important medical features and heart disease are explored through:

* Histograms
* Count Plots
* Box Plots
* Distribution Analysis

Key features analyzed include:

* Age
* Maximum Heart Rate (thalach)
* Chest Pain Type (cp)
* Exercise-Induced Angina (exang)

---

## ⚙️ Data Preprocessing

To prepare data for machine learning models, the following preprocessing steps are performed:

### Handling Missing Values

Numerical Features:

* Mean Imputation

Categorical Features:

* Most Frequent Value Imputation

### Feature Transformation

Numerical Features:

* Standard Scaling

Categorical Features:

* One-Hot Encoding

### Pipeline Implementation

Scikit-Learn Pipelines are used to automate:

* Data preprocessing
* Feature transformation
* Model training

Benefits:

* Cleaner workflow
* Reduced data leakage
* Better reproducibility

---

## 🤖 Machine Learning Models

The project compares multiple classification algorithms.

### 1. Logistic Regression

A baseline linear classification model used for binary prediction tasks.

**Advantages:**

* Fast training
* Easy interpretation
* Good baseline performance

---

### 2. Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees.

**Advantages:**

* Handles non-linear relationships
* Reduces overfitting
* Provides feature importance scores

---

### 3. Support Vector Machine (SVM)

A powerful classification algorithm that identifies the optimal decision boundary between classes.

**Advantages:**

* Effective in high-dimensional spaces
* Strong classification performance

---

### 4. K-Nearest Neighbors (KNN)

A distance-based classification algorithm that predicts based on neighboring data points.

**Advantages:**

* Simple and intuitive
* No training assumptions

---

## 📈 Model Evaluation

The models are evaluated using multiple classification metrics.

### Evaluation Metrics

#### Accuracy

Measures overall prediction correctness.

#### Precision

Measures how many predicted positive cases are actually positive.

#### Recall

Measures how many actual positive cases are correctly identified.

#### F1 Score

Balances Precision and Recall.

#### Confusion Matrix

Provides detailed insight into:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

## 🏆 Best Performing Model

Based on overall performance metrics:

| Rank | Model | Accuracy |
|------|--------|----------|
| 🥇 1 | Support Vector Machine (SVM) | **59%** |
| 🥈 2 | Logistic Regression | **58%** |
| 🥈 2 | K-Nearest Neighbors (KNN) | **58%** |
| 🥉 3 | Random Forest | **56%** |

### Key Takeaway

Among all evaluated models, **Support Vector Machine (SVM)** achieved the highest prediction accuracy (**59%**) and demonstrated the most balanced performance across Precision, Recall, and F1-Score. Therefore, SVM was selected as the best-performing model for this heart disease prediction task.

---

## 🔍 Feature Importance Analysis

One of the key strengths of the Random Forest model is its ability to identify the most influential features.

### Top Contributing Features

The project identifies important predictors such as:

* ca (Number of Major Vessels)
* thalach (Maximum Heart Rate)
* thal (Thalassemia Type)
* cp (Chest Pain Type)

A feature importance visualization is generated to understand the contribution of each feature.

---

## 📊 Key Findings

### Medical Insights

* Patients with lower maximum heart rates tend to have a higher likelihood of heart disease.
* Certain chest pain types show stronger associations with heart disease.
* The number of major vessels is one of the strongest predictors.
* Thalassemia-related measurements significantly influence predictions.

### Model Insights

* Random Forest demonstrated the strongest overall performance.
* SVM provided competitive classification results.
* Logistic Regression served as a useful baseline.
* KNN offered a simple yet effective alternative.

---

## 🚀 How to Run the Project

### Clone Repository

```bash
git clone https://github.com/yourusername/Heart-Disease-Predictor.git
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Heart_Disease_Predictor.ipynb
```

Run all cells sequentially.

---

## 📁 Project Structure

```text
Heart_Disease_Predictor/

│
├── Heart_Disease_Predictor.ipynb
├── README.md
│
└── Dataset (Downloaded via KaggleHub)
```

---

## 📚 Skills Demonstrated

This project showcases practical skills in:

* Machine Learning
* Classification Algorithms
* Data Preprocessing
* Feature Engineering
* Exploratory Data Analysis (EDA)
* Model Evaluation
* Scikit-Learn Pipelines
* Data Visualization
* Healthcare Analytics

---

## 🔮 Future Enhancements

Potential improvements include:

* Hyperparameter Tuning
* Cross Validation
* XGBoost Implementation
* LightGBM Implementation
* Model Deployment with Streamlit
* Real-Time Patient Prediction Interface
* Explainable AI (SHAP/LIME)

---

## 👩‍💻 Author

**Sakshi Srivastav**

Aspiring Data Scientist | Machine Learning Enthusiast | AI Developer

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

