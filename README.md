# Machine Learning Homework 2024

Author: Arianna Rigamonti

## Description
This project focuses on predicting taxonomic identity and genetic composition based on codon usage bias levels. The dataset, sourced from Khomtchouk, Bohdan B. *“Codon usage bias levels predict taxonomic identity and genetic composition”* (bioRxiv, 2020), includes codon usage frequencies from multiple organisms.

The goal is to classify organisms based on codon usage and recover missing feature data using machine learning techniques.

## Dataset
The dataset consists of 13,028 organisms and features two classification tasks:
1. **Kingdom classification** – Classifying organisms into 11 taxonomic groups.
2. **DNA type classification** – Identifying DNA types across 11 categories.

### Features:
- **67 attributes per sample**, including codon frequencies.
- **Training set:** 10,422 samples (`train.csv`).
- **Test set:** 2,606 samples (`test.csv`, missing AGA codon frequency).

## Tasks
1. **Data Analysis & Clustering**:
   - Visualizing data distribution.
   - Identifying feature correlations.
   - Evaluating clustering methods.

2. **Classification**:
   - Feature selection.
   - Model comparison (e.g., decision trees, SVMs, neural networks).
   - Testing on the provided test set.

3. **Regression for Missing Data**:
   - Training a regressor to predict missing AGA codon frequency.
   - Comparing regression algorithms.

4. **Evaluating the Impact of Missing Data Recovery**:
   - Retraining the classification model after imputing the missing AGA codon values.
   - Assessing performance improvements.

## Implementation
- **Language:** Python
- **Libraries Used:** `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`
- **Notebook:** The analysis and models are implemented in a Jupyter Notebook.

## Results
The project evaluates clustering, classification, and regression methods based on accuracy, precision, recall, and other relevant metrics. The final performance is assessed before and after imputing missing values.

## Usage
To reproduce the results:
1. Install dependencies:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```
2.	Run the Jupyter Notebook:
```bash
jupyter notebook MachineLearning_hw.ipynb
```
