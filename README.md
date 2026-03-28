# 🔊 Sonar Signal Classification (Rock vs Mine)

## 📌 Project Overview
This project focuses on classifying underwater sonar signals into:
- **Rock (R)**
- **Mine (M)**

The model analyzes sonar wave reflections and predicts whether the object is a rock or a mine using Machine Learning.

---

## 🌊 About Sonar
Sonar (Sound Navigation and Ranging) is a technique that uses sound waves to detect objects underwater. :contentReference[oaicite:0]{index=0}  

It works by sending sound signals and analyzing the reflected waves to identify objects.

---

## 📊 Dataset Information
- Total samples: **208**
- Features: **60 numerical attributes**
- Target:
  - `R` → Rock  
  - `M` → Mine  

Each feature represents the **energy of sonar signals at different frequency bands** :contentReference[oaicite:1]{index=1}  

---

## 🛠️ Technologies Used
- Python 🐍
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## ⚙️ Project Workflow

### 1. Data Loading
- Loaded dataset using Pandas

### 2. Data Preprocessing
- Checked for missing values
- Converted categorical labels to numerical

### 3. Exploratory Data Analysis (EDA)
- Visualized distributions using histograms
- Analyzed feature patterns

### 4. Train-Test Split
- Split dataset into training and testing sets

### 5. Model Training
- Used Machine Learning algorithm:
  - **Support Vector Machine (SVM)**

### 6. Model Evaluation
- Evaluated using accuracy score

---

## 📈 Results
- Achieved accuracy of approximately **90–95%**
- Model successfully classifies sonar signals

---

## 🔍 Example Prediction

```python
input_data = (your input values here)
prediction = model.predict(input_data)

if prediction[0] == 'R':
    print("Rock")
else:
    print("Mine")