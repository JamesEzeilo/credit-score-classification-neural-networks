# Credit Score Classification with Logistic Regression and Neural Networks

This project compares logistic regression and deep neural network (DNN) approaches for binary credit-score classification. It was completed as an independent academic assignment and is shared as a learning portfolio project.

## Project overview

The notebook builds and evaluates four models:

- Logistic regression without regularization
- Logistic regression with L2 regularization
- Deep neural network without regularization
- Deep neural network with L2 regularization, batch normalization, and dropout

Models are assessed using accuracy, precision, recall, F1 score, classification reports, and confusion matrices.

## Results

On the held-out test set used in the notebook, the non-regularized DNN achieved the strongest reported performance:

| Model | Accuracy | Precision | Recall | F1 score |
| --- | ---: | ---: | ---: | ---: |
| Logistic regression, no regularization | 92.53% | 93.45% | 91.40% | 92.41% |
| Logistic regression, L2 regularization | 92.42% | 93.36% | 91.27% | 92.30% |
| DNN, no regularization | 93.70% | 95.27% | 91.92% | 93.56% |
| DNN, with regularization | 93.44% | 95.15% | 91.49% | 93.28% |

## Repository contents

- `Assignment 2 - James Ezeilo.ipynb` — the current assignment notebook, including preprocessing, model training, evaluation, and visualisations
- `requirements.txt` — Python package dependencies
- `data/README.md` — local dataset setup notes

## Getting started

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Place the required CSV files in the same local directory as the notebook.
5. Open the notebook with Jupyter Notebook or JupyterLab and run the cells.

## Data

The underlying CSV files are not included in this repository. See `data/README.md` for the expected filenames and local setup instructions.

## Important note

This repository is a portfolio demonstration of machine-learning modelling and evaluation. It is not production credit-decision software and should not be used to make lending decisions.

## Next steps

A cleaned portfolio version will be added in a future update. Planned improvements include reproducible data handling, a consistent decision threshold, clearer model-selection rationale, and more deployment-oriented documentation.
