# 🧬 Scientific Abstract Classifier (NLP)

## 📖 Overview

A Machine Learning and Natural Language Processing (NLP) project that classifies scientific abstracts into three medical domains:

* 🩺 Cardiology
* 🧠 Neurology
* 🎗️ Cancer

The project demonstrates an end-to-end text classification workflow using **Python**, **Scikit-Learn**, and **TF-IDF Vectorization**, from data generation to model evaluation.

---

## ✨ Features

* Generate a synthetic dataset of scientific abstracts
* Perform text preprocessing and feature extraction
* Convert text into numerical vectors using TF-IDF
* Train a Logistic Regression classifier
* Evaluate model performance using:

  * Accuracy Score
  * Classification Report
  * Confusion Matrix
* Visualize results with heatmaps

---

## 📂 Repository Structure

```text
scientific-abstract-classifier/
│
├── scientific_abstracts.csv        # Generated dataset
├── Task7_Text_Classifier.ipynb     # Main Jupyter Notebook
├── README.md                       # Project documentation
└── requirements.txt                # Project dependencies (optional)
```

---

## 🏗️ Project Workflow

### 1️⃣ Data Collection

A balanced synthetic dataset of **100 scientific abstracts** was generated to simulate real-world medical research papers.

**Categories:**

* Cancer
* Neurology
* Cardiology

---

### 2️⃣ Text Preprocessing & Feature Engineering

The textual abstracts are transformed into numerical representations using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

TF-IDF helps:

* Highlight important domain-specific keywords
* Reduce the impact of common words
* Improve classification performance

**Example Keywords:**

| Domain     | Keywords                      |
| ---------- | ----------------------------- |
| Cancer     | tumor, oncology, chemotherapy |
| Neurology  | neuron, synapse, brain        |
| Cardiology | heart, artery, cardiovascular |

---

### 3️⃣ Model Training

**Algorithm:** Logistic Regression

Why Logistic Regression?

* Efficient for text classification
* Works well with sparse TF-IDF features
* Fast training and prediction

**Train-Test Split**

* Training Data: 80%
* Testing Data: 20%

---

## 📊 Results

### Model Performance

The classifier is evaluated on unseen test data using:

* Accuracy Score
* Precision
* Recall
* F1-Score

Example:

```text
Accuracy: 95%

Classification Report:
              precision    recall    f1-score
Cancer          0.95       0.96       0.95
Neurology       0.94       0.93       0.93
Cardiology      0.96       0.95       0.95
```

---

### Confusion Matrix

A confusion matrix heatmap is generated to visualize model predictions.

**Interpretation:**

* Strong diagonal values indicate correct predictions.
* Minimal off-diagonal values indicate low misclassification.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🚀 Installation & Usage

### Clone the Repository

```bash
git clone https://github.com/MuhammadHassanminhas/scientific-abstract-classifier.git
cd scientific-abstract-classifier
```

### Install Dependencies

```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
```

### Launch Jupyter Notebook

```bash
jupyter notebook Task7_Text_Classifier.ipynb
```

### Run the Notebook

Execute all cells to:

1. Generate the dataset
2. Preprocess text data
3. Train the classifier
4. Evaluate model performance
5. Display visualizations

---

## 📈 Future Improvements

* Increase dataset size using real PubMed abstracts
* Experiment with advanced NLP models

  * Naive Bayes
  * Support Vector Machines (SVM)
  * Random Forest
  * BERT / BioBERT
* Add model deployment using Flask or Streamlit
* Implement hyperparameter tuning

---

## 🤝 Contributing

Contributions are welcome!

Feel free to fork the repository, create a feature branch, and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Ibtisam Imtiaz**

GitHub: https://github.com/codeby-ibtisam

---

⭐ If you found this project useful, consider giving it a star on GitHub!
