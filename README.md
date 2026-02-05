# Customer Churn - CML (Simple)

This project trains a customer churn classifier using a Random Forest and compares three imbalance strategies: no adjustment, class weights, and SMOTE oversampling. It saves F1 scores and confusion matrices as outputs.

## Files
- `script.py` runs the full training/evaluation flow.
- `dataset.csv` is the input dataset.
- `requirements.txt` lists Python dependencies.

## Setup
1. Create and activate a virtual environment.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Run
```bash
python script.py
```

## Outputs
- `metrics.txt` with F1 scores for train and validation.
- `conf_matrix.png` combined confusion matrices for the three strategies.

## Notes
- The script drops `RowNumber`, `CustomerId`, and `Surname`.
- Rows with `Age > 80` are removed before training.
