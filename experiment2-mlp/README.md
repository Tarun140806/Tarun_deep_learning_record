# Experiment 2 — Multi-Layer Perceptron for Multi-Class Image Classification

**Course:** CS3807 — Deep Learning Laboratory, AY 2026–27
**Institution:** Shiv Nadar University Chennai, B.Tech AI & Data Science

## Objective

Build a Multi-Layer Perceptron (MLP) using TensorFlow/Keras and train it to classify
Fashion-MNIST images into one of ten clothing categories, including image preprocessing,
model construction, training, evaluation, and automated hyperparameter optimization.

## Dataset

- **Name:** Fashion-MNIST
- **Source:** Ships directly with Keras (`tensorflow.keras.datasets.fashion_mnist`) — no manual download required
- **Training images:** 60,000
- **Testing images:** 10,000
- **Classes:** 10 (T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)
- **Image size:** 28×28 grayscale

## Repository Contents

| File                                   | Description                                                                                      |
| -------------------------------------- | ------------------------------------------------------------------------------------------------ |
| `experiment_2_mlp_fashion_mnist.ipynb` | Full notebook: EDA, preprocessing, MLP construction, training, evaluation, hyperparameter search |
| `requirements.txt`                     | Python dependencies                                                                              |

The full LaTeX lab report (PDF) is submitted separately per course requirements and links back to this repository for source code.

## Dependencies

See `requirements.txt`. Install with:

```bash
pip install -r requirements.txt
```

## How to Run

1. Open `experiment_2_mlp_fashion_mnist.ipynb` in Jupyter or Google Colab.
2. Run all cells top to bottom. The dataset is fetched automatically via Keras.
3. Outputs include: sample images, class distribution, training/validation accuracy and loss curves, test-set accuracy/precision/recall/F1, confusion matrix, and hyperparameter search results.

**Note on hyperparameter search:** due to Colab compute-time constraints, `RandomizedSearchCV`'s `n_iter` was reduced to 3 (from a larger originally planned value). This is discussed explicitly in the report.

## Key Results

| Metric    | Baseline | Optimized |
| --------- | -------- | --------- |
| Accuracy  | 0.8919   | 0.8828    |
| Precision | 0.8950   | 0.8829    |
| Recall    | 0.8919   | 0.8828    |
| F1-score  | 0.8927   | 0.8825    |

## Author

Tarun K N — Shiv Nadar University Chennai
