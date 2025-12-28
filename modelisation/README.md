<p align="center">
  <img src="https://img.shields.io/github/license/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform?style=for-the-badge" />
  <img src="https://img.shields.io/badge/School%20Project-ML%20Modeling-blueviolet?style=for-the-badge" />
</p>

<h1 align="center">✨ Sentiment Analysis – Modeling ✨</h1>

<div align="center">
  <em>
     *Forging predictive models through data, experiments, and iteration*
  </em>
</br>

 <b>Model training, evaluation, and experiment tracking for a sentiment analysis pipeline</b>
</br>
</br>
🗃️ **Task**
  
    Binary sentiment classification (positive vs negative)

</div>

---

## 🎯 About This Module

This directory contains all elements related to **model experimentation and training** for the sentiment analysis project.

The objective is to:
- Explore multiple modeling approaches
- Compare classical machine learning and deep learning models
- Track experiments and metrics using MLflow
- Select a performant and deployable model for production

---

## 🗺️ Directory Structure

    modelisation/
    ├── notebooks/                # Exploration & training notebooks
    │   ├── modelisation.ipynb
    │   ├── final_model_tf.ipynb
    │   └── Nettoyage.ipynb
    │
    ├── mlruns/                   # MLflow experiment tracking
    │
    ├── distilbert_model.tflite   # Exported production-ready model
    ├── requirements.txt          # Modeling dependencies
    └── README.md

---

## 🪄 Models Tested

| Model                    | Description |
|--------------------------|-------------|
| TF-IDF + LogisticRegression | Strong linear baseline on sparse features |
| LSTM                     | Recurrent neural network capturing word order |
| CNN                      | Convolutional model extracting local n-gram patterns |
| CNN + LSTM               | Hybrid architecture (convolution + temporal memory) |
| DistilBERT               | Lightweight transformer with contextual embeddings |

---

## 👑 Key Results

| Model                | F1-Score | Accuracy | ROC AUC |
|----------------------|----------|----------|---------|
| TF-IDF + LogReg      | 0.73     | 0.72     | 0.79    |
| LSTM                 | 0.61     | 0.54     | 0.58    |
| CNN                  | 0.63     | 0.59     | 0.64    |
| CNN + LSTM           | 0.58     | 0.50     | 0.52    |
| DistilBERT           | **0.78** | **0.79** | **0.87** |

All experiments and metrics are tracked via **MLflow**.

---

## 🧙 Experiment Tracking with MLflow

To inspect experiments and compare runs visually:

1. Open a terminal at the project root
2. Launch the MLflow UI:

    mlflow ui

The MLflow interface will be available locally at:

    http://localhost:5000

---

## 🔮 Model Selection

**DistilBERT** was selected as the final model due to:
- Best overall performance across metrics
- Strong generalization capability
- Compatibility with TensorFlow Lite for deployment
- Reasonable inference cost for production use

The exported model is stored as:

    distilbert_model.tflite

---

## ✒️ License

This modeling work is provided for educational purposes only.

<p align="right">(<a href="#top">back to top</a>)</p>

---

## 🕊️ Contact

Joëlle JEAN BAPTISTE  
LinkedIn:

    https://fr.linkedin.com/in/joëllejnbaptiste

Project Repository:

    https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform

<p align="right">(<a href="#top">back to top</a>)</p>
