<h1 align="center">📰 Fake News Classifier using LSTM</h1>

<p align="center">
  <em>A Deep Learning-based approach to classify news articles as <b>Real</b> or <b>Fake</b> using LSTM (Long Short-Term Memory) Networks.</em>
</p>

---

## 📘 Project Overview
This project demonstrates the power of **Natural Language Processing (NLP)** and **Deep Learning** for fake news detection.  
It uses an **LSTM neural network** built with **TensorFlow/Keras** to classify news articles based on their titles or text content as *Real* or *Fake*.

The model learns contextual word dependencies by analyzing text sequences, making it more robust than traditional machine learning models like Naive Bayes or Logistic Regression.

---

## 🧠 Problem Statement
In the digital era, fake news spreads rapidly through online platforms and social media.  
Detecting such misinformation is crucial to maintaining public trust and data authenticity.  
This project aims to automate fake news detection using an **LSTM-based deep learning model** trained on a labeled dataset of real and fake news.

---

## 🧩 Dataset
- **File used:** `Fake_news.csv`  
- The dataset contains:
  - `title` → headline of the news article  
  - `label` → `1` for real news, `0` for fake news  

You can use your own dataset or download a similar one from Kaggle:  
👉 [Kaggle Fake News Dataset](https://www.kaggle.com/c/fake-news)

---

## ⚙️ Workflow

### 🧹 Step 1: Data Preprocessing
- Loaded the dataset using **Pandas**
- Removed missing/null values
- Cleaned text using **Regex**
- Tokenized and converted to lowercase
- Removed **stopwords**
- Applied **stemming** using `PorterStemmer`
- Encoded words using **One-Hot Encoding**
- Padded sequences to fixed length (20 words)

### 🧱 Step 2: Model Architecture
The deep learning model consists of:

**Loss Function:** `binary_crossentropy`  
**Optimizer:** `adam`  
**Metric:** `accuracy`

### 🧪 Step 3: Training
- Model was trained on preprocessed sequences
- Achieved high accuracy and generalization performance
- Used **Sequential API** from Keras for model building

---

## 📈 Results

| Metric | Value |
|:-------:|:------:|
| Training Accuracy | ~95% |
| Validation Accuracy | ~93% |
| Loss Function | Binary Crossentropy |
| Model Type | LSTM (Sequential) |

Example Predictions:

