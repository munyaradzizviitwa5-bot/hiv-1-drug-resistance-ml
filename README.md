
# Machine Learning-Based Prediction and Interpretability of HIV-1 Drug Resistance Across Antiretroviral Classes Using Viral Genomic Sequences

## 1. Project Overview

HIV-1 drug resistance is a major challenge in the effective treatment and long-term management of HIV infection. Genetic mutations in the HIV-1 genome can alter the virus's susceptibility to antiretroviral drugs, potentially reducing treatment effectiveness.

This project investigates the application of machine learning techniques to predict HIV-1 antiretroviral drug resistance using viral genetic sequence and mutation-related data.

The study focuses on examining relationships between HIV-1 genetic variation and phenotypic drug susceptibility, developing predictive models, evaluating their performance, and exploring model interpretability.

The overall aim is to reproduce and extend a data-driven HIV-1 drug-resistance prediction workflow using reproducible computational methods.

**Project status:** Ongoing — data exploration, preprocessing, and reproduction of the initial analysis are the current priorities.

---

## 2. Research Objectives

The main objectives of this project are to:

1. Explore and characterize HIV-1 genotype–phenotype data.
2. Investigate the relationship between viral genetic mutations and antiretroviral drug susceptibility.
3. Perform data cleaning, preprocessing, and feature engineering.
4. Develop machine learning models for predicting HIV-1 drug resistance.
5. Evaluate model performance using appropriate classification and statistical metrics.
6. Investigate model interpretability to identify genetic features associated with resistance predictions.
7. Establish a reproducible computational workflow that can be independently examined and further developed.

---

## 3. Dataset Description

The project uses an HIV-1 genotype–phenotype dataset containing viral sequence identifiers, patient identifiers, subtype information, protease mutation features, and phenotypic susceptibility measurements for protease inhibitor (PI) antiretroviral drugs.

The dataset contains approximately:

- **4,350 observations**
- **116–119 variables**, depending on the version being examined
- Viral sequence and isolate identifiers
- Patient and HIV-1 subtype information
- Protease mutation features (P1–P99)
- A composite mutation-list field
- Phenotypic susceptibility measurements for multiple protease inhibitors

The eight protease inhibitor drugs represented include:

- Atazanavir (ATV)
- Darunavir (DRV)
- Fosamprenavir (FPV)
- Indinavir (IDV)
- Lopinavir (LPV)
- Nelfinavir (NFV)
- Saquinavir (SQV)
- Tipranavir (TPV)

### Dataset Source

The dataset appears to correspond to genotype–phenotype data associated with the **Stanford HIV Drug Resistance Database (HIVDB)**.

The original source and applicable data-use or redistribution conditions will be verified and documented before the dataset is publicly redistributed.

**Note:** The raw dataset is not included in this repository at present. This repository will document the dataset source and provide instructions for obtaining the data where permitted.

---

## 4. Methodology

The project will follow a structured computational workflow.

### 4.1 Data Exploration

- Inspect dataset dimensions and variable types.
- Examine missing values and duplicate observations.
- Investigate repeated patient and sequence identifiers.
- Explore HIV-1 subtype distribution.
- Examine the distribution of phenotypic susceptibility measurements.
- Assess the availability of phenotype measurements across antiretroviral drugs.

### 4.2 Data Preprocessing

- Handle missing values using scientifically justified methods.
- Investigate duplicate and repeated records.
- Prepare genotype and phenotype features for modelling.
- Examine class imbalance.
- Define appropriate prediction targets.
- Preserve the original dataset and document all transformations.

### 4.3 Feature Engineering

Potential features include:

- Protease mutation indicators.
- HIV-1 subtype information.
- Mutation combinations.
- Other relevant genotype-related variables.

Feature selection and encoding methods will be documented to support reproducibility.

### 4.4 Machine Learning Development

Candidate machine learning approaches may include:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting methods

The final models will depend on the structure of the data, the research objectives, and the results of model evaluation.

### 4.5 Model Evaluation

Model performance will be assessed using appropriate metrics, which may include:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrices

Validation procedures will be selected carefully. Where patient identifiers permit, patient-level grouping will be considered to reduce the risk of data leakage between training and testing sets.

### 4.6 Model Interpretability

Interpretability methods, potentially including feature importance and SHAP (SHapley Additive exPlanations), will be investigated to understand which genetic features contribute to model predictions.

---

## 5. Tools and Technologies

The project uses or plans to use the following technologies:

| Tool / Technology | Purpose |
|---|---|
| Python | Data analysis and machine learning |
| Google Colab | Cloud-based computational environment |
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning and model evaluation |
| SHAP | Model interpretability |
| Git and GitHub | Version control and project documentation |

Additional tools may be introduced as the project develops.

---

## 6. Repository Structure

The repository is being organized using the following structure:

```text
hiv-1-drug-resistance-ml/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   └── README.md
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_model_training.ipynb
│   ├── 05_model_evaluation.ipynb
│   └── 06_model_interpretability.ipynb
│
├── src/
│   └── preprocessing.py
│
├── results/
│
└── docs/
    └── methodology.md
```

*The structure will be populated progressively as the project develops.*

---

## 7. Reproducibility and Research Practices

Reproducibility is a central priority of this project.

The following practices will be followed:

- Preserve the original dataset without modifying it.
- Document data-cleaning and preprocessing procedures.
- Maintain organized Jupyter notebooks.
- Record software dependencies and relevant package versions.
- Use appropriate training, validation, and testing procedures.
- Document model configurations and evaluation metrics.
- Maintain version history through Git and GitHub.
- Avoid publishing restricted, sensitive, or personally identifiable information.

The aim is to make the computational workflow transparent and easier for other researchers to understand and reproduce, subject to dataset access and licensing conditions.

---

## 8. Current Project Status

The project is currently in development.

| Research Component | Status |
|---|---|
| GitHub repository creation | Completed |
| Initial dataset inspection | Completed |
| Data exploration | In progress |
| Data preprocessing | Planned / in progress |
| Feature engineering | Planned |
| Machine learning development | Planned |
| Model evaluation | Planned |
| Model interpretability | Planned |
| Final documentation | Planned |

Project status will be updated as each stage is completed and verified.

---

## 9. Expected Research Contribution

This project aims to demonstrate how computational biology and machine learning can be applied to HIV-1 genotype–phenotype data.

The expected outcomes include:

- A documented and reproducible data-analysis workflow.
- An investigation of genetic features associated with antiretroviral drug susceptibility.
- Machine learning models for selected drug-resistance prediction tasks.
- Evaluation of model performance and limitations.
- An interpretable analysis of genetic features influencing predictions.

The project is intended as an academic research and learning exercise. Its predictive models are not intended for clinical diagnosis or treatment decisions.

---

## 10. Limitations

Potential limitations include:

- Missing phenotypic measurements for some drugs.
- Unequal representation of drug-resistance categories.
- Repeated patient or sequence identifiers.
- Differences in HIV-1 subtype representation.
- Limitations in the availability and quality of genotype–phenotype observations.
- Potential differences between the dataset's original experimental methods and the intended modelling approach.

These limitations will be investigated and reported during the analysis.

---

## 11. Researcher

**Biotechnology Undergraduate Student | Galgotias University**

Academic interests:

- Bioinformatics
- Computational Biology
- Genomics
- Molecular Biology
- Artificial Intelligence in Biomedical Research
- Machine Learning in Healthcare and Biological Data Analysis

Currently developing practical skills in Python, R, statistics, data analysis, and machine learning, with a long-term academic interest in computational approaches to understanding biological systems and disease-associated genetic variation.

---

## 12. References and Acknowledgements

The dataset attribution and relevant scientific references will be documented as the original source and associated publications are verified.

**Potential resource for dataset documentation:**

- Stanford HIV Drug Resistance Database (HIVDB): https://hivdb.stanford.edu/

All dataset use, attribution, and redistribution will follow the applicable source terms and permissions.

---

## 13. Disclaimer

This repository is intended for academic, educational, and research purposes only.

The analyses and predictive models developed in this project are experimental and should not be interpreted as clinical recommendations or used to make individual patient treatment decisions.
