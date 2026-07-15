# Experiment 1 — Single Layer Perceptron for Binary Classification

**Course:** CS3807 — Deep Learning Laboratory, AY 2026–27
**Institution:** Shiv Nadar University Chennai, B.Tech AI & Data Science

## Objective

Implement a Single Layer Perceptron from scratch to perform binary classification
on the UCI Banknote Authentication dataset, and evaluate it using standard
classification metrics.

## Dataset

- **Name:** Banknote Authentication Dataset
- **Source:** UCI Machine Learning Repository — https://archive.ics.uci.edu/dataset/267/banknote+authentication
- **Instances:** 1372
- **Features:** variance, skewness, curtosis, entropy (4 numerical features, extracted from wavelet-transformed banknote images)
- **Classes:** 0 = Authentic, 1 = Forged
- **Missing values:** None

The dataset is fetched automatically inside the notebook via the `ucimlrepo`
package — no manual download required.

## Repository Contents

| File                        | Description                                                                        |
| --------------------------- | ---------------------------------------------------------------------------------- |
| `perceptron_banknote.ipynb` | Full notebook: EDA, preprocessing, perceptron implementation, training, evaluation |
| `epoch_wise_learning.csv`   | Epoch-wise training log (misclassified count, weights, bias per epoch)             |
| `report/report.pdf`         | Full lab report (compiled)                                                         |
| `report/report.tex`         | LaTeX source for the report                                                        |
| `report/figures/`           | Generated plots (EPS, 600 DPI)                                                     |
| `requirements.txt`          | Python dependencies                                                                |

## Dependencies

See `requirements.txt`. Install with:

```bash
pip install -r requirements.txt
```

## How to Run

1. Open `perceptron_banknote.ipynb` in Jupyter or Google Colab.
2. Run all cells top to bottom. The dataset is fetched automatically via `ucimlrepo`.
3. Outputs include: EDA plots, trained perceptron weights/bias per epoch,
   test-set accuracy/precision/recall/F1, and the confusion matrix.

## Key Results

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 0.9891 |
| Precision | 0.9837 |
| Recall    | 0.9918 |
| F1-score  | 0.9878 |

## Author

Tarun K N — Shiv Nadar University Chennai
