<p align="center">
  <img src="https://img.shields.io/github/license/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform?style=for-the-badge" />
  <img src="https://img.shields.io/badge/School%20Project-ML%20%26%20Frontend-blueviolet?style=for-the-badge" />
</p>

<h1 align="center">✨ Sentiment Analysis Frontend ✨</h1>

<div align="center">
  <em>
     *A lightweight magical interface to interrogate machine learning predictions*
  </em>
</br>

 <b>Streamlit frontend used to interact with a sentiment analysis API and collect user feedback</b>
</br>
</br>
🔮 **Backend API**
  
    Sentiment Analysis FastAPI (see /back)

</div>

---

## ✨ Features

- Send free text to a sentiment analysis API
- Display predictions (positive / negative)
- Collect user feedback on predictions
- Forward corrections back to the backend API

---

## 🗺️ Project Structure

    front/
    ├── app.py                # Streamlit application
    ├── requirements.txt      # Frontend dependencies
    └── README.md

---

## ⚔️ Getting Started

### 1. Clone the repository

    git clone https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform.git
    cd SchoolProject---End-to-end-sentiment-analysis-platform/front

### 2. Create and activate a virtual environment

    python -m venv .venv

    # On Windows
    .venv\Scripts\activate

    # On macOS / Linux
    source .venv/bin/activate

### 3. Install dependencies

    pip install -r requirements.txt

---

## 🪄 Run the Application

Start the Streamlit app:

    streamlit run app.py

The application will be available locally at:

    http://localhost:8501

---

## 🧙 Notes

- The backend API **must be running and accessible**
- The API URL is configured inside the Streamlit app
- SSL verification is disabled **only for local testing**
- Do **not** use `verify=False` in production environments

---

## ✒️ License

This frontend is provided for educational purposes only.

<p align="right">(<a href="#top">back to top</a>)</p>

---

## 🕊️ Contact

Joëlle JEAN BAPTISTE  
LinkedIn:

    https://fr.linkedin.com/in/joëllejnbaptiste

Project Repository:

    https://github.com/joelle-jnbaptiste/SchoolProject---End-to-end-sentiment-analysis-platform

<p align="right">(<a href="#top">back to top</a>)</p>
