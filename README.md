# CDC Diabetes Dataset - Individual Assignment

This repository contains Jupyter notebooks for exploring, modeling, and explaining diabetes-related outcomes using the CDC BRFSS dataset. It is written to be accessible for readers with different backgrounds and focuses on clear, reproducible analysis.

## What You Will Find

- Exploratory analysis of the dataset and class imbalance
- Binary and 3-class classification models
- Imbalance handling (balanced weights, SMOTE)
- Model tuning (GridSearchCV, Optuna)
- Explainability (feature importance, SHAP)
- Association rule mining for risk factor patterns
- Clustering analyses for population segmentation

## Dataset

- Source: CDC Behavioral Risk Factor Surveillance System (BRFSS)
- File: CDC Diabetes Dataset.csv
- Target: Diabetes_012
  - 0 = No diabetes
  - 1 = Prediabetes
  - 2 = Diabetes

## Notebooks (Suggested Order)

1. Classification_Model_Binary.ipynb
   - Binary classification: No diabetes vs Prediabetes/Diabetes
2. Classification_Model_3_Categories.ipynb
   - 3-class classification for Diabetes_012
3. AssociationRuleDimensionReduction.ipynb
   - Association rules on engineered binary features
4. Clustering_Model.ipynb
   - Clustering analysis
5. K-Means_Approach.ipynb
   - Alternative clustering workflow
6. Draft.ipynb
   - Scratchpad and experiments

## Setup

1. Optional: create a virtual environment
   - Windows PowerShell:
     - python -m venv .venv
     - .\.venv\Scripts\Activate.ps1

2. Install packages
   - pip install -r requirements.txt

## How to Run

- Open the notebooks in VS Code or Jupyter.
- Run cells top to bottom in each notebook.
- Long-running steps (Optuna, SHAP, Apriori) can be reduced by lowering trials or sampling the data.

## Notes on Reproducibility

- Random seeds are set in several sections, but results can still vary slightly due to stochastic algorithms.
- If you see a NumPy/Numba compatibility error with SHAP, pin NumPy to <= 2.3.

## Responsible Use

This project is for learning and analysis only. It does not provide medical advice. Use results responsibly and validate against clinical guidance before any real-world decisions.

## Contact

If you have questions or need clarification, please open an issue or add a note to your report.
