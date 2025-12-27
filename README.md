<!-- Improved compatibility of back to top link -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
<div align="center">

[![Stars][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

</div>


<!-- PROJECT LOGO -->
<br />
<div align="center">

<h3 align="center">🧙‍♂️ End-to-End Sentiment Analysis Platform</h3>

<p align="center">
  A full sentiment analysis platform, from raw data to deployed prediction service, blending data science, machine learning, and MLOps into a single production-ready pipeline.
  <br />
  <br />
  <strong>📜 School Project — Machine Learning & Engineering</strong>
  <br />
  <br />
  <a href="https://www.kaggle.com/datasets/kazanova/sentiment140"><strong>📚 Dataset (Sentiment140) »</strong></a>
  <br />
  <br />
  <a href="https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform">🗡️ Project Repository</a>
</p>
</div>

---

<!-- TABLE OF CONTENTS -->
<details>
  <summary>📜 Grimoire of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">🔮 About The Project</a>
      <ul>
        <li><a href="#context">🧩 Context</a></li>
        <li><a href="#objectives">🎯 Objectives</a></li>
      </ul>
    </li>
    <li><a href="#architecture-overview">🏰 Architecture Overview</a></li>
    <li><a href="#project-structure">🗂️ Project Structure</a></li>
    <li><a href="#data">📊 Dataset</a></li>
    <li><a href="#built-with">✨ Built With</a></li>
    <li><a href="#models">🤖 Models & Experiments</a></li>
    <li><a href="#api">🧪 Prediction API</a></li>
    <li><a href="#frontend">🖥️ Frontend Interface</a></li>
    <li><a href="#mlops">⚙️ MLOps & Automation</a></li>
    <li><a href="#roadmap">🗺️ Roadmap</a></li>
    <li><a href="#license">📄 License</a></li>
    <li><a href="#contact">📬 Contact</a></li>
  </ol>
</details>

---

## 🔮 About The Project

This repository unifies **three previously independent projects** into a single **end-to-end sentiment analysis platform**:

- 📖 Data exploration & cleansing  
- 🧠 Model training & comparison  
- 🧪 API deployment for inference  
- 🖥️ Frontend for real-time usage  
- ⚙️ Monitoring, testing, and automation  

The focus is not only on model accuracy, but on **building a complete, production-ready ML system**.

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---
### ✨ Built With

#### 🧙 Core Language
![Python](https://img.shields.io/badge/Python-4B0082?style=for-the-badge&logo=python&logoColor=FFD700)

#### 🔮 Machine Learning & NLP
![TensorFlow](https://img.shields.io/badge/TensorFlow-6A0DAD?style=for-the-badge&logo=tensorflow&logoColor=FFD700)
![Keras](https://img.shields.io/badge/Keras-5D3FD3?style=for-the-badge&logo=keras&logoColor=FFD700)
![TensorFlow Lite](https://img.shields.io/badge/TensorFlow_Lite-7B2CBF?style=for-the-badge&logo=tensorflow&logoColor=FFD700)
![DistilBERT](https://img.shields.io/badge/DistilBERT-3A0CA3?style=for-the-badge&logo=huggingface&logoColor=FFD700)

#### 🏰 Backend & API
![FastAPI](https://img.shields.io/badge/FastAPI-3A0CA3?style=for-the-badge&logo=fastapi&logoColor=FFD700)

#### 🪄 Frontend
![Streamlit](https://img.shields.io/badge/Streamlit-7209B7?style=for-the-badge&logo=streamlit&logoColor=FFD700)

#### 📜 Experiment Tracking & Monitoring
![MLflow](https://img.shields.io/badge/MLflow-560BAD?style=for-the-badge&logo=mlflow&logoColor=FFD700)

#### ⚔️ DevOps & Deployment
![Docker](https://img.shields.io/badge/Docker-4B0082?style=for-the-badge&logo=docker&logoColor=FFD700)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-5A189A?style=for-the-badge&logo=githubactions&logoColor=FFD700)


---

### 🧩 Context

You play the role of a **Data Scientist / ML Engineer** commissioned to design a sentiment analysis tool based on social media content.

The solution must be:

- 🪄 Interpretable  
- 🛡️ Reliable  
- ⚙️ Deployable  
- 🧑‍💼 Usable by non-technical stakeholders  

This project mirrors real-world ML constraints encountered in industry.

---

### 🎯 Objectives

- Build and compare several sentiment classification models  
- Track experiments and metrics  
- Deploy the best model behind an API  
- Provide a simple frontend for interaction  
- Capture user feedback to monitor prediction quality  

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 🏰 Architecture Overview

The platform follows a classic **ML production pipeline**:

- 📊 **Data Layer** — ingestion, cleaning, feature engineering  
- 🧠 **Modeling Layer** — experimentation and selection  
- 🧪 **Serving Layer** — API for inference and feedback  
- 🖥️ **Interface Layer** — user interaction  
- ⚙️ **MLOps Layer** — tracking, tests, CI/CD  

Each component is isolated yet connected, ensuring **clarity, modularity, and scalability**.

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 🗂️ Project Structure

```text
SchoolProject---End-to-end-sentiment-analysis-platform/
│
├── modelisation/
│   ├── Nettoyage.ipynb
│   ├── modelisation.ipynb
│   ├── final_model_tf.ipynb
│   ├── mlruns/
│   └── README.md
│
├── api/
│   ├── main.py
│   └── model_final/
│       ├── distilbert_model.tflite
│       └── model_loader.py
│
├── front/
│   ├── app.py
│   └── README.md
│
├── .github/workflows/
│   ├── tests.yml
│   └── deploy.yml
│
├── Dockerfile
├── requirements.txt
└── README.md
```
<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>
## 📊 Dataset

### 📚 Sentiment140

- **Source**: Kaggle  
- **Dataset**: Sentiment140  
- **Lien**: https://www.kaggle.com/datasets/kazanova/sentiment140  

**Description du grimoire de données** 🪄  
Le dataset **Sentiment140** contient environ **1,6 million de tweets** annotés automatiquement selon leur polarité :

- `0` → sentiment négatif  
- `4` → sentiment positif  

Chaque entrée comprend notamment :
- le texte brut du tweet
- un identifiant
- des métadonnées temporelles

Ces données reflètent un **langage réel, bruité et non structuré**, proche des cas industriels.

---

### 📜 Référence méthodologique

La démarche initiale d’exploration et de modélisation s’inspire de l’article Kaggle suivant, servant de **point d’entrée pédagogique** :

- https://www.kaggle.com/code/kazanova/sentiment140  

Ce projet va toutefois **au-delà** de ce kernel en intégrant :
- une vraie séparation entraînement / service
- une API de prédiction
- un frontend utilisateur
- des briques MLOps

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---


## 🤖 Models & Experiments

Plusieurs créatures algorithmiques ont été invoquées avant d’élire le champion final :

- 🧪 **TF-IDF + Logistic Regression**  
  Modèle linéaire robuste servant de baseline.

- 🧠 **LSTM**  
  Capte la dynamique séquentielle des phrases.

- 🕸️ **CNN**  
  Détecte des motifs locaux (n-grams).

- 🔗 **CNN + LSTM**  
  Architecture hybride.

- 👑 **DistilBERT**  
  Modèle final retenu pour son excellent compromis performance / complexité.

### 🧾 Suivi des expériences

Toutes les expériences sont tracées avec **MLflow** :
- métriques (accuracy, F1-score, ROC-AUC)
- paramètres
- artefacts modèles

Les logs sont disponibles dans le dossier `modelisation/mlruns/`.

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 🧪 Prediction API

La couche service est assurée par une **API FastAPI**, conçue comme un artefact de production.

### 🔮 Fonctionnalités

- Chargement du modèle **DistilBERT (TFLite)**
- Prédiction de sentiment à partir d’un texte
- Enregistrement du feedback utilisateur

### 🗝️ Endpoints principaux

- `POST /predict` → prédiction du sentiment  
- `POST /feedback` → retour utilisateur  

### 🐳 Exécution via Docker

    docker build -t sentiment-api .
    docker run -p 8000:8000 sentiment-api

Une fois lancée, la documentation interactive est accessible sur :

    http://localhost:8000/docs

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 🖥️ Frontend Interface

Un **grimoire d’invocation visuel** a été conçu avec **Streamlit**.

### 🪄 Fonctionnalités

- Saisie d’un texte libre
- Appel de l’API de prédiction
- Affichage du sentiment (positif / négatif)
- Envoi d’un feedback utilisateur

### 🚀 Lancer l’interface

    streamlit run app.py

L’application s’ouvre par défaut sur :

    http://localhost:8501

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## ⚙️ MLOps & Automation

Ce projet met l’accent sur les **bonnes pratiques industrielles** :

- 🧪 Tests unitaires (modèle & API)
- 🔁 CI avec GitHub Actions
- 📜 Versionnement des modèles
- 🐳 Environnements reproductibles

L’objectif est de démontrer une **chaîne ML complète**, fiable et maintenable.

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 🗺️ Roadmap

Améliorations futures envisagées :

- 🔍 Explicabilité des prédictions (SHAP / LIME)
- 🧿 Détection de dérive de données
- 🔁 Ré-entraînement automatique basé sur le feedback
- ☁️ Déploiement cloud (Azure / GCP)
- 🌍 Support multilingue

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 📄 License

Ce projet est fourni **à des fins pédagogiques** dans le cadre d’une formation en data science.  
L’utilisation des données est soumise aux conditions de Kaggle.

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>

---

## 📬 Contact

🧙‍♀️ **Joëlle JEAN BAPTISTE**  
🔗 LinkedIn : https://fr.linkedin.com/in/joëllejnbaptiste  

🗡️ Project Repository :  
https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform

<p align="right">(<a href="#readme-top">🔝 back to top</a>)</p>
<!-- MARKDOWN LINKS & IMAGES -->

[stars-shield]: https://img.shields.io/github/stars/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform.svg?style=for-the-badge
[stars-url]: https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform/stargazers

[issues-shield]: https://img.shields.io/github/issues/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform.svg?style=for-the-badge
[issues-url]: https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform/issues

[license-shield]: https://img.shields.io/badge/License-Educational-6A0DAD?style=for-the-badge
[license-url]: #

[linkedin-shield]: https://img.shields.io/badge/LinkedIn-4B0082?style=for-the-badge&logo=linkedin&logoColor=FFD700
[linkedin-url]: https://fr.linkedin.com/in/jo%C3%ABllejnbaptiste



