# Practical 03 – Data Pre-processing

**Course:** ML6402 – Machine Learning  
**Instructor:** Dr. Ahmed Sabbah

This practical accompanies Lecture 3 and focuses on turning raw data into a reproducible machine-learning workflow.

## Main topics

- Loading and inspecting a dataset
- Missing values
- Feature/target separation
- Train/test split
- Data leakage
- Numeric imputation
- Categorical encoding
- Standardization and normalization
- `ColumnTransformer`
- `Pipeline`
- Reproducible preprocessing
- Student exercises and challenge tasks

## Files

- `ML6402_Practical03_Data_Preprocessing.ipynb` – guided Jupyter notebook
- `data/salary.csv` – small preprocessing dataset used in the guided example

## Run with Anaconda

From the repository root:

```bash
conda activate ml6402
jupyter notebook
```

Then open this folder and run the notebook from top to bottom.

## Learning principle

Preprocessing is part of the experimental design. Any transformation that learns from data must be fitted using the training set only and then applied to unseen data.
