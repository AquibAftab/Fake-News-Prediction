# 📘 Fake News Detection Using Machine Learning

This project focuses on building a **Fake News Detection System** using **Machine Learning (Logistic Regression)** with complete **data cleaning, preprocessing, TF-IDF feature extraction, and model prediction**.

It also provides a **user input prediction** feature and displays **similar true news articles** to help with credibility verification.

---

## 📌 Project Overview

Fake news has become a major challenge in the digital era. The aim of this project is to:

* Detect whether a news article is **REAL** or **FAKE**.
* Use **Logistic Regression** for classification.
* Use **TF-IDF Vectorization** for text data.
* Perform full **text preprocessing**.
* Provide a **Jupyter Notebook implementation**.

---

## 📂 Dataset Used

We used the **True.csv** and **Fake.csv** datasets from Kaggle.

* **True.csv** → Collection of verified real news
* **Fake.csv** → Collection of fabricated or fake news

Each dataset contains:

* `title` (may be empty)
* `text` (primary data used)
* `subject`
* `date`

We add a new column:

* `label = 1` → Real News
* `label = 0` → Fake News

---

## 🧹 Data Cleaning & Preprocessing

To prepare the text for ML modeling, the following steps were applied:

### ✔ 1. Lowercasing

```
"This is NEWS" → "this is news"
```

### ✔ 2. Remove URLs

### ✔ 3. Remove Numbers

### ✔ 4. Remove Punctuation

### ✔ 5. Remove Stopwords

### ✔ 6. Tokenization

### ✔ 7. Lemmatization

```
"running" → "run"
"better" → "good"
```

### ✔ 8. Remove Duplicate News

### ✔ 9. Remove Null Records

---

## 🔧 Machine Learning Pipeline

Below is the complete pipeline followed:

### **1️⃣ Load Dataset**

Combine TRUE and FAKE datasets into one.

### **2️⃣ Clean the Text**

Apply preprocessing using NLTK tools.

### **3️⃣ Split Dataset**

Training: 80%
Testing: 20%

### **4️⃣ TF-IDF Vectorization**

Convert text → numerical vectors.

### **5️⃣ Train Logistic Regression Model**

A simple yet powerful linear classifier.

### **6️⃣ Predict on New Input**

User can type any news article.

### **7️⃣ Show Similar True News**

Top 5 news articles displayed using cosine similarity.

---

## 📊 Model Evaluation (Highlighted Metrics Added)

### ⭐ **Important Model Metrics (Highlighted):**

* **✔ Accuracy Score** – Measures overall correctness of the model.
* **✔ F1 Score** – Balances Precision and Recall; best metric for Fake News classification.

These two metrics are essential for evaluating the quality and reliability of the Fake News Detection model.

After training, the model is evaluated using **accuracy**.

Typical results:

* Accuracy: **92% – 98%**
* Logistic Regression performs strongly with TF-IDF.

---

## 📷 Figures & Workflow Diagrams

### 🖼 **Figure 1: Project Workflow**

```
Dataset → Cleaning → Vectorization → Model Training → Prediction → Output
```

### 🖼 **Figure 2: Text Preprocessing Pipeline**

```
Raw Text → Lowercase → Remove Noise → Tokenize → Lemmatize → Clean Text
```

### 🖼 **Figure 3: Machine Learning Pipeline**

```
TF-IDF → Logistic Regression → Accuracy Score → User Prediction
```

---

## 💻 Running the Project in Jupyter Notebook

### Step 1: Install Dependencies

```bash
pip install nltk scikit-learn pandas numpy
```

### Step 2: Upload `True.csv` and `Fake.csv` into the notebook.

### Step 3: Run the Notebook Cells

Cells include:

* Import libraries
* Cleaning functions
* Vectorization
* Training model
* Prediction function

### Step 4: Use the Predictor

User enters:

```
"NASA released a statement confirming a new discovery on Mars."
```

Model responds TRUE or FAKE.

---

## 🧪 Example Output

```
Enter news article:
"Government announces free healthcare starting next year"

🔴 Result: The news is MOST LIKELY FAKE.

Similar TRUE news:
1. (Example true article...)
2. ...
```

---

## 📦 Folder Structure

```
📁 Fake-News-Detection
│
├── 📄 README.md
├── 📄 Fake.ipynb
├── 📄 True.csv
├── 📄 Fake.csv
└── 📄 requirements.txt
```

---

## 🚀 Future Improvements

* Use **BERT or RoBERTa** for higher accuracy
* Add **web interface (Streamlit)**
* Add **fake image detection**
* Deploy using **Flask / FastAPI**

---

## 🧑‍💻 Author

Aquib Aftab

If you'd like, I can also create:

* A **PPT presentation**
* A **PDF project report**
* A **GitHub README version**
* A **Streamlit Web App**

