
# 🧬 Scientific Abstract Classifier (NLP)

**Task 7: ML Text Classification**
An end-to-end Machine Learning pipeline that classifies scientific abstracts into three medical domains: **Cancer, Neurology, and Cardiology**. Built using Python, Scikit-Learn, and TF-IDF vectorization.

## 📌 Project Overview

This project demonstrates a complete NLP workflow designed to categorize medical text data.

1.  **Data Generation:** Creates a synthetic dataset of 100 scientific abstracts.
2.  **Preprocessing:** Cleans and converts text to numerical vectors using **TF-IDF**.
3.  **Modeling:** Trains a **Logistic Regression** classifier.
4.  **Evaluation:** Validates performance using Accuracy scores and Confusion Matrices.

-----

## 📂 Repository Structure

```text
.
├── scientific_abstracts.csv    # (Generated) The dataset used for training
├── Task7_Text_Classifier.ipynb # Main Jupyter Notebook containing all code         
└── README.md                   # Project documentation
```

-----

## 🚀 Workflow Steps

### 1\. Data Collection

We generated a balanced dataset containing 100 synthetic abstracts.

  * **Source:** Python generation script (simulating PubMed-style text).
  * **Classes:** `Cancer`, `Neuro`, `Cardio`.

### 2\. Feature Engineering

Text data was transformed using **TF-IDF (Term Frequency-Inverse Document Frequency)**. This technique converts raw text into numerical features, highlighting domain-specific keywords like *"tumor"* or *"synapse"* while ignoring common stopwords.

### 3\. Model Training

  * **Algorithm:** Logistic Regression (chosen for its efficiency with sparse text data).
  * **Split:** 80% Training / 20% Testing.

-----

## 📊 Results & Visualization

### **Model Performance**

The model was evaluated on a held-out test set (20% of data). The Classification Report below details the Precision, Recall, and F1-Scores for each category.

### **Confusion Matrix**

The heatmap below visualizes the model's predictions versus the actual labels. The strong diagonal line indicates high classification accuracy across all three categories.

-----

## 🛠️ How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/codeby-ibtisam/scientific-abstract-classifier.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas scikit-learn matplotlib seaborn jupyter
    ```
3.  **Launch the Notebook:**
    ```bash
    jupyter notebook Task7_Text_Classifier.ipynb
    ```
4.  **Run All Cells:**
    The notebook is self-contained. Running all cells will generate the dataset, train the model, and display the output plots.



## 📜 License

This project is open-source and available under the MIT License.
