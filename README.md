# Statistical Analysis and Structure Discovery in Wine Quality Data

## Foundations of Statistical Modelling (MDE-CS-03)

### Constructor University — Spring 2026

**Author:** Subhankar Biswas
**Matriculation Number:** 30008967
**Course:** MDE-CS-03 Principles of Statistical Modelling
**Instructor:** Prof. Dr. Stefan Kettemann

---

## Project Overview

This project presents a comprehensive statistical analysis of the Wine Quality dataset obtained from the UCI Machine Learning Repository.

The objective is to identify and characterize statistical structures in physicochemical wine measurements using techniques introduced in the Foundations of Statistical Modelling course.

The project combines:

* Distribution Analysis
* Probability Mass Functions (PMFs)
* Moment Analysis
* Distribution Fitting
* Correlation Analysis
* Joint Probability Mass Functions
* Bivariate Gaussian Modeling
* Principal Component Analysis (PCA)
* Linear Regression
* Outlier Detection

---

## Dataset

**Dataset:** Wine Quality Dataset (Red Wine)

Source:

(https://archive.ics.uci.edu/dataset/186/wine+quality)

Original publication:

P. Cortez, A. Cerdeira, F. Almeida, T. Matos, J. Reis,
*Modeling wine preferences by data mining from physicochemical properties*,
Decision Support Systems, Vol. 47, pp. 547–553 (2009).

Dataset Characteristics:

| Property        | Value     |
| --------------- | --------- |
| Samples         | 1599      |
| Features        | 11        |
| Target Variable | Quality   |
| Type            | Numerical |

---

## Repository Structure

```text
PSM-Wine-Quality-Analysis/
│
├── raw-data/
│   └── winequality-red.csv
│
├── Output (Plots)/
│   ├── histogram.png
│   ├── pmf.png
│   ├── distribution_fit.png
│   ├── scatter.png
│   ├── heatmap.png
│   ├── joint_pmf.png
│   ├── gaussian_surface.png
│   ├── pca_variance.png
│   └── pca_scatter.png
│
├── Report & Presentations/
│   └── PSM_Project_Report__Statistical_Structure_Analysis_of_the_Wine_Quality_Dataset.pdf
│
├── Wine_Quality_Data.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Mathematical Formalism

Let

Ω = {ω₁, ω₂, ..., ωₙ}

denote the universe of wine samples.

Each sample is represented by a random vector:

X = (X₁, X₂, ..., X₁₁)

where the variables correspond to physicochemical wine properties such as acidity, density, sulphates, and alcohol content.

The data value space is defined as:

S = S₁ × S₂ × ... × S₁₁

with:

Xᵢ : Ω → Sᵢ

---

## Statistical Methods

### Exercise Sheet 5

* Histogram Estimation
* Probability Mass Functions
* Mean Estimation
* Standard Deviation
* Skewness
* Kurtosis
* Gaussian Distribution Fitting
* Gamma Distribution Fitting
* RMSE Comparison

### Exercise Sheet 6

* Scatter Plots
* Pearson Correlation Coefficient
* Cross-Correlation Matrix
* Joint PMF Estimation
* Covariance Analysis
* Bivariate Gaussian Modeling

### Project Extension

* Principal Component Analysis (PCA)
* Explained Variance Analysis
* Linear Regression
* Outlier Detection

---

## Key Findings

### Distribution Analysis

* Alcohol content exhibits positive skewness.
* Gamma distribution provides a better fit than the Gaussian model.

### Correlation Analysis

* Alcohol and density show significant negative correlation.
* Several physicochemical variables exhibit strong dependencies.

### Principal Component Analysis

* A small number of principal components explain a large fraction of total variance.
* The dataset exhibits latent low-dimensional structure.

### Regression Analysis

* Wine quality can be partially predicted from physicochemical properties.
* Linear relationships explain part of the observed variability.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Subiswas36218/PSM-Wine-Quality-Analysis.git
cd PSM-Wine-Quality-Analysis
```

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Wine_Quality_Data.ipynb
```

Run all cells sequentially.

---

## License

This repository is submitted as coursework for:

**MDE-CS-03 Principles of Statistical Modelling**
**Constructor University**
**Spring 2026**
