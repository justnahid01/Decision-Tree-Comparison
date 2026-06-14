# Decision Tree Comparison: CART vs ID3

## Project Overview

This project compares two popular Decision Tree algorithms:

* CART (Classification and Regression Tree)
* ID3 (Iterative Dichotomiser 3)

The objective is to evaluate and compare their classification performance using a common dataset and multiple evaluation metrics.

---

## Dataset

Dataset Source:

DT_Dataset.csv

Target Variable:

* Approved

The dataset contains both numerical and categorical features.

---

## Project Workflow

### 1. Data Exploration (EDA)

The dataset was examined using:

* Dataset overview
* Missing value analysis
* Duplicate record analysis
* Descriptive statistics
* Feature distributions
* Correlation analysis
* Outlier detection

### 2. Data Preprocessing

#### Missing Value Handling

Missing numerical values were imputed using the median strategy.

#### Categorical Encoding

Categorical features were transformed using Label Encoding.

#### Feature Scaling

Data was standardized using StandardScaler.

#### Data Splitting

* Training Set: 70%
* Testing Set: 30%

---

## Model Development

### CART Model

Criterion:

Gini Index

### ID3 Model

Criterion:

Entropy

---

## Hyperparameter Optimization

GridSearchCV was used with 5-fold cross-validation.

Parameters Tested:

* max_depth = [3, 5, 7, 10, None]
* min_samples_split = [2, 5, 10, 20]

The best-performing configuration for each algorithm was automatically selected.

---

## Visualizations

### Decision Boundary Visualization

PCA was used to reduce dimensionality for 2D visualization.

### Confusion Matrix

Heatmaps were generated for both models.

### ROC Curve

Receiver Operating Characteristic curves were plotted and compared.

### Evaluation Metrics

The following metrics were evaluated:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Results

Both CART and ID3 models were trained and evaluated under identical conditions.

Performance was compared using:

* Classification Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

This comparison provides insight into how different splitting criteria influence decision tree performance.

---

## Repository Structure

dataset/
DT_Dataset.csv

notebook/
Decision_Tree_Comparison.ipynb

README.md

---

## Author

Nahid Hasan
