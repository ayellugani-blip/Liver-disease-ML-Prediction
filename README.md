# 🩺 Liver Disease Prediction Using Machine Learning

A machine learning classification project that uses patient health records and liver function test parameters to predict whether a patient is likely to have liver disease.

## 📌 Project Overview

Liver disease can be difficult to identify in its early stages. This project explores how machine learning can identify patterns in patient records and support the classification of patients as liver patients or non-liver patients.

The project uses the **Indian Liver Patient Dataset (ILPD)** and follows a standard machine learning workflow: dataset understanding, data preprocessing, exploratory data analysis (EDA), class-imbalance handling, model development, and model evaluation.

> **Important:** This is an academic project. Its predictions are not a medical diagnosis and must not replace advice, examination, or treatment from a qualified healthcare professional.

## 🎯 Objectives

- Understand the Indian Liver Patient Dataset and its target variable.
- Clean and preprocess the patient records.
- Explore feature distributions and relationships through EDA.
- Address class imbalance using an appropriate approach.
- Train and evaluate classification models.
- Compare model performance and justify the final model selection using evaluation results.

## 📂 Dataset

**Dataset:** Indian Liver Patient Dataset (ILPD)  
**Source:** Kaggle (originally from the UCI Machine Learning Repository)

[View and download the dataset on Kaggle](https://www.kaggle.com/datasets/uciml/indian-liver-patient-records)

| Dataset detail | Description |
|---|---|
| Records | 583 |
| Input features | 10 |
| Target column | 1 |
| Numerical input features | 9 |
| Categorical input features | 1 (Gender) |
| Task | Binary classification |

### Target variable

The dataset's `Dataset` column uses these labels:

- `1` — Liver patient
- `2` — Non-liver patient

### Input features

| Feature | Description |
|---|---|
| Age | Patient age |
| Gender | Patient gender |
| Total_Bilirubin | Total bilirubin level |
| Direct_Bilirubin | Direct bilirubin level |
| Alkaline_Phosphotase | Alkaline phosphatase (ALP) level |
| Alamine_Aminotransferase | Alanine aminotransferase (ALT) level |
| Aspartate_Aminotransferase | Aspartate aminotransferase (AST) level |
| Total_Protiens | Total protein level |
| Albumin | Albumin level |
| Albumin_and_Globulin_Ratio | Albumin-to-globulin ratio |

## 🔬 Methodology

The planned workflow is:

1. **Dataset identification** — obtain the ILPD dataset.
2. **Dataset understanding** — inspect the records, attributes, data types, and target labels.
3. **Data cleaning and preprocessing** — check missing values, duplicates, data types, and outliers.
4. **Exploratory data analysis** — use descriptive statistics and visualizations to study the data.
5. **Feature preparation** — encode Gender and prepare the target labels; apply scaling where required.
6. **Class-imbalance handling** — consider SMOTE or class weights, applying resampling only to the training data.
7. **Train-test split** — use stratified sampling to preserve class proportions.
8. **Model development** — train the proposed classifiers.
9. **Model evaluation and comparison** — compare models using consistent evaluation metrics.
10. **Result interpretation** — discuss model strengths, limitations, and the selected model.

## 📊 Exploratory Data Analysis

The project EDA covers:

- Descriptive statistics (mean, median, minimum, maximum, and standard deviation).
- Histograms and box plots for feature distributions.
- Class distribution of liver and non-liver patients.
- Feature comparisons across the target classes.
- Age-wise and gender-wise analysis.
- Correlation heatmap and pair plots for selected features.

Visualizations are created using Matplotlib and Seaborn.

## 🤖 Machine Learning Models

The synopsis proposes the following classification algorithms:

| Model | Purpose |
|---|---|
| Decision Tree | An interpretable tree-based baseline classifier. |
| Random Forest | An ensemble of decision trees for more stable predictions. |
| Naive Bayes | A probabilistic classifier used as a comparison model. |

The final model should be selected based on the measured evaluation results rather than assumed in advance.

## 📈 Evaluation Metrics

Because the dataset is imbalanced, accuracy alone may not adequately describe model performance. The project considers:

- **Precision** — proportion of predicted positive cases that are actually positive.
- **Recall** — proportion of actual positive cases correctly identified.
- **F1-score** — harmonic mean of precision and recall.
- **Confusion matrix** — counts of correct and incorrect predictions.
- **Accuracy and ROC-AUC** — additional performance measures.

Model comparisons should use the same train-test split and evaluation metrics for a fair comparison.

## 🛠️ Tools and Technologies

| Tool / Library | Purpose |
|---|---|
| Python | Programming language |
| NumPy | Numerical operations |
| Pandas | Data handling and analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning and evaluation |
| imbalanced-learn | Class-imbalance handling |
| Jupyter Notebook / Google Colab | Development environment |
| Git and GitHub | Version control |

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ayellugani-blip/Liver-disease-ML-Prediction.git
cd Liver-disease-ML-Prediction
```

### 2. Set up Python

Create and activate a virtual environment (recommended):

```bash
python -m venv .venv
```

On Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

Install the libraries used by the project:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

### 4. Open the notebook

Start Jupyter:

```bash
jupyter notebook
```

Open the project's `.ipynb` notebook and run its cells in order.

**Dataset note:** Download the ILPD dataset from the Kaggle link above and place the CSV file at the path expected by the notebook. Update the notebook's dataset path if you store the file elsewhere.

## 📁 Repository Contents

The main project notebook is intended to contain the end-to-end analysis and model development. Add or update this section as files are committed so that the list reflects the repository's actual contents.

## 👥 Team Members

| Team Member | Responsibility |
|---|---|
| K. Karthik Varma | Dataset Understanding, Preprocessing & EDA |
| Y. Anudeep | Model Development & Evaluation |
| U. Varun | Model Comparison, Documentation & Presentation |

## 📚 References

1. [Indian Liver Patient Dataset — Kaggle](https://www.kaggle.com/datasets/uciml/indian-liver-patient-records)
2. [UCI Machine Learning Repository](https://archive.ics.uci.edu/)
3. [Scikit-learn Documentation](https://scikit-learn.org/stable/)
4. [imbalanced-learn Documentation](https://imbalanced-learn.org/stable/)
5. [Pandas Documentation](https://pandas.pydata.org/docs/)
6. [NumPy Documentation](https://numpy.org/doc/)
7. [Matplotlib Documentation](https://matplotlib.org/stable/)
8. [Seaborn Documentation](https://seaborn.pydata.org/)

## ⚠️ Disclaimer

This project is developed for educational purposes as part of a Project Based Learning activity. It is not a clinically validated diagnostic system. Do not use its predictions to make healthcare decisions; consult a qualified medical professional for diagnosis and treatment.
