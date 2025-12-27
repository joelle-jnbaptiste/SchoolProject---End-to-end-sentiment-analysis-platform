# Sentiment Analysis – Modeling

This directory contains scripts, trained models, visualizations, and results related to the **sentiment classification** of tweets (binary: *positive* vs *negative*) for a machine learning project.

---

## Directory Structure

- `notebooks/` – exploratory and training notebooks
- `mlruns/` – MLflow logs for experiment tracking

---

## Models Tested

| Model                      | Description |
|---------------------------|-------------|
| `TF-IDF + LogisticRegression` | Simple yet robust linear model, performs well on sparse features |
| `LSTM`                    | RNN that captures word sequence and temporal dynamics |
| `CNN`                     | Captures local patterns in sequences (e.g., n-grams) |
| `CNN + LSTM`              | Hybrid architecture combining convolution and memory |
| `DistilBERT`              | Lightweight pre-trained transformer model with contextual embeddings |

---

## Key Results

| Model              | F1-Score | Accuracy | ROC AUC |
|-------------------|----------|----------|---------|
| TF-IDF + LogReg   | 0.73     | 0.72     | 0.79    |
| LSTM              | 0.61     | 0.54     | 0.58    |
| CNN               | 0.63     | 0.59     | 0.64    |
| CNN + LSTM        | 0.58     | 0.50     | 0.52    |
| **DistilBERT**    | **0.78** | **0.79** | **0.87** |

> All experiment logs are tracked via `MLflow` in the `mlruns/` folder

---

## Running MLflow

To inspect experiment metrics and comparisons visually:

1. Open a terminal at the project root
2. Launch the MLflow UI server:

```bash
mlflow ui
