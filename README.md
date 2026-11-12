# Project presentation

Dataset reference : Bani, Z. (2023). An open‑access dataset of emergency department admissions at a large teaching hospital in Iran. Data Archiving and Networked Services (DANS). https://doi.org/10.17632/vhzyyktrz5.

The project aims at predicting hospitalisation ``DischargeFromED`` from triage (I may look to spot the hospital stays that may be extended in the future).

# Key steps

- **Data pre-processing**: Cleaning, selecting variables prior to hospitalisation and encoding.
- **Exploratory Data Analysis (EDA)**: Statistical visualisations of the target (DischargeFromED) and boxplot, correlation matrix of numerical values.
- **Modelling & evaluation**: Training linear (SGD Classifier) and non-linear (HGB Classifier, XGBoost) models. Evaluation from ``classification_report`` and confusion matrices.

# Results

At the moment, XGBoost and HGB Classifier performed the best (0.82 accuracy). They are closely followed by the SGD Classifier (0.77 accuracy).

Limits are the data only comes from one hospital in Iran, during the Covid-19 epidemic. We assumed we had access to ``ChiefComplaint`` and could convert it to CIM-10's notation 1st letter automatically, in a similar manner to humans.

# Packages

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn