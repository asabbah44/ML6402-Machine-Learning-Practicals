# Practical 04 – Regression I: Simple Linear Regression

**Course:** ML6402 – Machine Learning  
**Instructor:** Dr. Ahmed Sabbah

This practical is intended to be both a laboratory activity and a self-study resource.

## Structure

### Part A – Understand the model

Students study:

- regression intuition;
- the regression equation;
- intercept and slope;
- predictions and residuals;
- squared error;
- the cost function;
- cost-versus-parameter plots;
- Gradient Descent;
- learning rate and convergence.

### Part B – Build the model

Students then apply the ideas to the 30-observation stipend dataset using Scikit-Learn:

- inspect the dataset;
- visualize the relationship;
- define X and y;
- split train/test;
- fit `LinearRegression`;
- inspect learned parameters;
- predict unseen observations;
- analyze residuals;
- calculate MAE, MSE, RMSE, and R²;
- compare with a mean baseline.

## Files

- `ML6402_Practical04_Simple_Linear_Regression.ipynb`
- `data/StipendData.csv`

## Running locally

From the repository root:

```bash
conda activate ml6402
jupyter notebook
```

Then open this folder and run the notebook from top to bottom.

## Google Colab

The notebook contains a second dataset-loading option for Colab. Comment the local loading lines and uncomment the GitHub URL lines as instructed in the notebook.
