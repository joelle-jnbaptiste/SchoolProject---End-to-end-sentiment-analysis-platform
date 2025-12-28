<p align="center">
  <img src="https://img.shields.io/github/license/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform?style=for-the-badge" />
  <img src="https://img.shields.io/badge/School%20Project-ML%20%26%20Data-blueviolet?style=for-the-badge" />
</p>

<h1 align="center">✨ End-to-End Sentiment Analysis Platform ✨</h1>

<div align="center">
  <em>
     *From raw text to real-time predictions*
  </em>
</br>

 <b>An end-to-end platform for sentiment analysis, covering data preparation, model training, deployment, monitoring, and user feedback</b>
</br>
</br>
🗃️ **Dataset**  
 https://www.kaggle.com/datasets/kazanova/sentiment140
  
</div>

---


<!-- TABLE OF CONTENTS -->
<details>
  <summary>🧭 Table of Contents</summary>
  <ol>
    <li><a href="#-built-with">Built With</a></li>
    <li><a href="#-about-the-project">About The Project</a></li>
    <li><a href="#-dataset">Dataset</a></li>
    <li><a href="#-architecture-overview">Architecture Overview</a></li>
    <li><a href="#-models--experiments">Models & Experiments</a></li>
    <li><a href="#-prediction-api">Prediction API</a></li>
    <li><a href="#-frontend-interface">Frontend Interface</a></li>
    <li><a href="#-mlops--automation">MLOps & Automation</a></li>
    <li><a href="#-repository-structure">Repository Structure</a></li>
    <li><a href="#-getting-started">Getting Started</a></li>
    <li><a href="#-license">License</a></li>
    <li><a href="#-contact">Contact</a></li>
  </ol>
</details>

---
### ✨ Built With

[![Python][Python-shield]][Python-url]
[![FastAPI][FastAPI-shield]][FastAPI-url]
[![Streamlit][Streamlit-shield]][Streamlit-url]
[![ScikitLearn][ScikitLearn-shield]][ScikitLearn-url]
[![MLflow][MLflow-shield]][MLflow-url]
[![Docker][Docker-shield]][Docker-url]
[![Azure][Azure-shield]][Azure-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🎯 About The Project

This project implements a **complete end-to-end sentiment analysis platform**, designed to reflect a **production-ready machine learning workflow**.

It covers the full lifecycle of an ML product:

- Data preparation and exploration
- Model training and comparison
- API deployment for real-time predictions
- User feedback collection
- Monitoring and automation using MLOps principles

The goal is to demonstrate how a sentiment analysis model can be **designed, deployed, and maintained** in a realistic environment.

---

## 🗃️  Dataset

The project uses the **Sentiment140** dataset, a widely used benchmark for sentiment analysis tasks.

- 1.6M labeled tweets
- Binary sentiment labels (positive / negative)
- Real-world, noisy text data

Dataset source:  
https://www.kaggle.com/datasets/kazanova/sentiment140

---

## 🏰 Architecture Overview

The platform follows a modular architecture:

- **Data layer**: preprocessing and dataset handling
- **Modeling layer**: training, evaluation, and explainability
- **API layer**: FastAPI service exposing prediction endpoints
- **Frontend layer**: Streamlit interface for interaction and validation
- **MLOps layer**: MLflow tracking, deployment automation, monitoring

This architecture emphasizes **scalability**, **traceability**, and **maintainability**.

---

## 🪄 Models & Experiments

Several models are explored and compared:

- Classical machine learning models
- Neural network-based approaches
- Transformer-based models

Experiments include:

- Feature engineering and text preprocessing
- Hyperparameter tuning
- Model comparison using standard NLP metrics
- Explainability analysis (feature importance / SHAP-style insights)

---

## 👑 Model Evaluation

Models are evaluated using:

- Accuracy
- Precision / Recall
- F1-score
- Error analysis on misclassified samples

Evaluation results are logged and tracked using **MLflow**.

---

## 🔮 Prediction API

A **FastAPI** service exposes the trained model for inference.

Main features:

- REST endpoints for predictions
- Input validation
- Logging of prediction outcomes
- Feedback loop for incorrect predictions

The API is containerized and deployable via Docker.

---

## 🖥️ Frontend Interface

A **Streamlit** application allows users to:

- Submit text for sentiment prediction
- Visualize prediction confidence
- Validate or reject model outputs
- Explore model behavior interactively

This interface closes the loop between users and the ML system.

---

## 🧪 MLOps & Automation

The project integrates key MLOps practices:

- Experiment tracking with MLflow
- Model versioning
- Deployment automation
- Monitoring prediction quality
- Alerting on degraded performance

The objective is to simulate **real-world ML operations**.

---

## 🗺️ Repository Structure

    SchoolProject---End-to-end-sentiment-analysis-platform/
    ├── api/                 # FastAPI service
    ├── frontend/            # Streamlit application
    ├── notebooks/           # Experiments & analysis
    ├── models/              # Trained models
    ├── docker/              # Docker configuration
    ├── mlflow/              # Experiment tracking
    └── README.md

---

## ⚔️ Getting Started

This project can be run locally using Docker or directly with Python.

### Prerequisites

- Python 3.9+
- Docker (optional)
- pip or conda

### Installation

1. Clone the repository:

       git clone https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform.git

2. Install dependencies:

       pip install -r requirements.txt

3. Launch the API:

       uvicorn api.main:app --reload

4. Launch the frontend:

       streamlit run frontend/app.py

---

## ✒️ License

This project is provided for educational purposes.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 🕊️ Contact

Joëlle JEAN BAPTISTE  
LinkedIn: https://fr.linkedin.com/in/joëllejnbaptiste  

Project Link: https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

[Python-shield]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://www.python.org/
[FastAPI-shield]: https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white
[FastAPI-url]: https://fastapi.tiangolo.com/
[Streamlit-shield]: https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white
[Streamlit-url]: https://streamlit.io/
[ScikitLearn-shield]: https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white
[ScikitLearn-url]: https://scikit-learn.org/
[MLflow-shield]: https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge
[MLflow-url]: https://mlflow.org/
[Docker-shield]: https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com/
[Azure-shield]: https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white
[Azure-url]: https://azure.microsoft.com/
