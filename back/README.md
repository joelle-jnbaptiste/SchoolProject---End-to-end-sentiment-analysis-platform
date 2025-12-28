<p align="center">
  <img src="https://img.shields.io/github/license/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform?style=for-the-badge" />
  <img src="https://img.shields.io/badge/School%20Project-ML%20%26%20Data-blueviolet?style=for-the-badge" />
</p>

<h1 align="center">✨ Sentiment Analysis API ✨</h1>

<div align="center">
  <em>
     *Turning text into predictions*
  </em>
</br>

 <b>A production-ready REST API for real-time sentiment analysis, built with FastAPI and a TensorFlow Lite NLP model</b>
</br>
</br>
🗃️ **Model**  
 DistilBERT (TensorFlow Lite)
  
</div>

---


<!-- TABLE OF CONTENTS -->
<details>
  <summary>🧭 Table of Contents</summary>
  <ol>
    <li><a href="#-built-with">Built With</a></li>
    <li><a href="#-about-the-api">About The API</a></li>
    <li><a href="#-architecture">Architecture</a></li>
    <li><a href="#-available-endpoints">Available Endpoints</a></li>
    <li><a href="#-project-structure">Project Structure</a></li>
    <li><a href="#-run-with-docker">Run with Docker</a></li>
    <li><a href="#-tests">Tests</a></li>
    <li><a href="#-license">License</a></li>
  </ol>
</details>

---
### ✨ Built With

[![Python][Python-shield]][Python-url]
[![FastAPI][FastAPI-shield]][FastAPI-url]
[![TensorFlow][TensorFlow-shield]][TensorFlow-url]
[![Docker][Docker-shield]][Docker-url]
[![Pytest][Pytest-shield]][Pytest-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🎯 About The API

This API provides **real-time sentiment prediction** for short text inputs.

It is part of the **End-to-End Sentiment Analysis Platform** and focuses on the **serving layer** of the machine learning system.

Key responsibilities:

- Load and serve a trained NLP model
- Expose prediction endpoints
- Log user feedback
- Enable automated testing and containerized deployment

The API is designed to be **lightweight**, **testable**, and **cloud-ready**.

---

## 🏰 Architecture

High-level flow:

1. Client sends a text input  
2. API preprocesses the text  
3. TensorFlow Lite model performs inference  
4. Prediction and confidence are returned  
5. Optional user feedback is stored for monitoring  

The model is loaded once at startup to minimize latency.

---
## 🪄 Available Endpoints

| Method | Endpoint     | Description                         |
|------:|--------------|-------------------------------------|
| POST  | `/predict`   | Predict sentiment from a text input |
| POST  | `/feedback`  | Submit user feedback on prediction  |

Interactive API documentation:

    http://localhost:8000/docs

---

## 🗺️ Project Structure

    back/
    ├── api/
    │   └── main.py              # FastAPI application
    │
    ├── model_final/
    │   ├── distilbert_model.tflite
    │   └── model_loader.py      # Model loading & inference logic
    │
    ├── tests/
    │   └── test_model.py        # Unit tests
    │
    ├── Dockerfile               # API containerization
    ├── requirements.txt         # Core dependencies
    ├── requirements-api.txt     # API-specific dependencies
    ├── pytest.ini               # Pytest configuration
    └── README.md

---

## 🧙‍♂️ Run with Docker

### 1. Build the Docker image

    docker build -t sentiment-api .

### 2. Run the container locally

    docker run -p 8000:8000 sentiment-api

Then access the API documentation:

    http://localhost:8000/docs

---

## 🧪 Tests

Unit tests are implemented using **pytest**.

Covered aspects:

- Model loading
- Positive / negative predictions
- Batch accuracy verification

Run tests locally:

    pytest

---

## ✒️ License

This project is provided for educational purposes.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
---

[Python-shield]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://www.python.org/
[FastAPI-shield]: https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white
[FastAPI-url]: https://fastapi.tiangolo.com/
[TensorFlow-shield]: https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white
[TensorFlow-url]: https://www.tensorflow.org/
[Docker-shield]: https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com/
[Pytest-shield]: https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge
[Pytest-url]: https://docs.pytest.org/
