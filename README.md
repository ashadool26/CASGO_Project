# CSGO Round Winner Prediction

A machine learning project that predicts the **round winner** in Counter-Strike: Global Offensive (CS:GO) using match-state telemetry data.

## Project Overview

This repository contains an end-to-end notebook workflow for:
- loading and cleaning CS:GO round data,
- encoding categorical features,
- training baseline and improved classifiers,
- applying **Linear Discriminant Analysis (LDA)** for feature selection,
- evaluating model performance with accuracy and confusion matrices.

The analysis is implemented in:
- `CSGO_Project_by_ashadool.ipynb`

## Dataset

- Dataset source (Google Drive):  
  <https://drive.google.com/file/d/1PMoa51-JvNZ_ar8ACQSw_6g9RJJd2LOQ/view?usp=sharing>
- Notebook-reported raw size: **122,410 rows × 97 columns**
- Missing values: none reported
- Duplicates: removed during preprocessing

## Workflow Summary

1. **Data Loading & Quality Checks**
   - Load CSV with pandas.
   - Inspect schema, descriptive statistics, nulls, and duplicates.

2. **Preprocessing**
   - Label-encode key categorical columns:
     - `bomb_planted`
     - `map`
     - `round_winner`
   - Split into training and test sets.

3. **Baseline Model**
   - Train Logistic Regression on full feature set.

4. **Feature Selection with LDA**
   - Standardize features with `StandardScaler`.
   - Fit LDA on training data.
   - Score features from `lda.coef_` and select top 20.

5. **Model Training on Selected Features**
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier

6. **Evaluation**
   - Compare models by test accuracy.
   - Review confusion matrices.

## Results

Notebook outputs report the following accuracies:

- Logistic Regression (without LDA): **74.25%**
- Logistic Regression (with LDA-selected features): **75.30%**
- Decision Tree (with LDA-selected features): **81.22%**
- Random Forest (with LDA-selected features): **85.50%** ✅

**Best-performing model:** Random Forest (after LDA-based feature selection).

## Tech Stack

- Python
- Jupyter Notebook / Google Colab
- pandas
- NumPy
- Matplotlib
- scikit-learn

## How to Run

1. Clone this repository.
2. Download the dataset from the link above.
3. Update the dataset path in the notebook (currently Colab-style path is used).
4. Open and run:
   - `CSGO_Project_by_ashadool.ipynb`

### Example local setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook
```

## Repository Structure

```text
.
├── CSGO_Project_by_ashadool.ipynb   # Main analysis and modeling notebook
└── README.md                        # Project documentation
```

## Future Improvements

- Add reproducible training scripts (`src/` + `requirements.txt`).
- Track experiments and hyperparameters.
- Add additional metrics (F1, ROC-AUC, precision/recall).
- Package the best model for inference.
- Build a small dashboard/API for live predictions.

## Author

Created by **Ashadool**.
