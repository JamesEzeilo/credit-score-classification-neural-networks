# Credit Score Classification with Logistic Regression and Neural Networks

This completed portfolio project compares logistic regression and deep neural network (DNN) approaches for binary credit-score classification. It was originally completed as an independent academic assignment and has been refactored into a reproducible portfolio implementation.

## Project overview

The cleaned notebook compares two models:

- Logistic regression with L2 regularization
- Deep neural network with L2 regularization, batch normalization, dropout, early stopping, and learning-rate reduction

Both models are assessed with accuracy, precision, recall, F1 score, confusion matrices, and DNN training-loss history.

## Repository contents

- `notebooks/credit_score_classification_clean.ipynb` — completed, cleaned portfolio notebook with reproducible preprocessing and model evaluation
- `Assignment 2 - James Ezeilo.ipynb` — original assignment notebook retained for reference
- `requirements.txt` — Python package dependencies
- `data/README.md` — local dataset setup instructions

## Reproducible methodology

The cleaned implementation:

- Derives the classification threshold from the training file only and applies it consistently to validation and test data.
- Fits median imputation and standardisation only on the training partition.
- Uses a dynamic input feature count rather than a hard-coded architecture input size.
- Keeps the test set held out until final evaluation.
- Uses a fixed random seed and validation-based callbacks for the DNN.

## Getting started

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Obtain the authorised CSV files and place them in the same local directory as the notebook.
5. Open `notebooks/credit_score_classification_clean.ipynb` with Jupyter Notebook or JupyterLab and run the cells.

## Data

The underlying CSV files are not included in this repository. They remain local because they are not cleared for redistribution here. See `data/README.md` for the expected filenames.

## Important note

This repository is a completed portfolio demonstration of machine-learning modelling and evaluation. It is not production credit-decision software and must not be used to make lending decisions. Any real-world credit-risk application would also require calibration, fairness, explainability, governance, stability, and regulatory assessment.
