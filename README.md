# 🧠 Sentiment Analysis using NLP & BiGRU

A deep learning-based **Sentiment Analysis application** that uses **Natural Language Processing (NLP)** and a **Bidirectional GRU (BiGRU)** neural network to classify text sentiment.

The trained model is exposed through a **FastAPI REST API**, allowing users to submit text and receive sentiment predictions through an easy-to-use interface.

## 🚀 Live Project

🔗 **GitHub Repository:**
https://github.com/MuskanPatel0027/Sentimental_Analysis_NLP

## 📌 Project Overview

Sentiment Analysis is an NLP task used to determine the emotional polarity of a piece of text.

This project processes user-provided text and predicts its sentiment using a deep learning model based on **Bidirectional GRU (BiGRU)**.

### Key capabilities

* 📝 Text preprocessing and cleaning
* 🔤 NLP-based text vectorization
* 🧠 Deep learning using BiGRU
* 📊 Sentiment classification
* ⚡ FastAPI REST API
* 🌐 Web-based interface
* 🚀 Deployment-ready configuration
* 📦 Model artifacts and preprocessing components

---

## 🏗️ Project Architecture

```text
                User Input
                    │
                    ▼
            ┌───────────────┐
            │   Web / API   │
            └───────┬───────┘
                    │
                    ▼
          ┌───────────────────┐
          │ Text Preprocessing│
          └─────────┬─────────┘
                    │
                    ▼
          ┌───────────────────┐
          │ Tokenization /    │
          │ Sequence Padding  │
          └─────────┬─────────┘
                    │
                    ▼
          ┌───────────────────┐
          │   BiGRU Model     │
          │ Deep Learning     │
          └─────────┬─────────┘
                    │
                    ▼
          ┌───────────────────┐
          │ Sentiment         │
          │ Prediction        │
          └─────────┬─────────┘
                    │
                    ▼
              API Response
```

---

## 🛠️ Tech Stack

| Technology          | Purpose                                |
| ------------------- | -------------------------------------- |
| Python              | Core programming language              |
| NLP                 | Text processing and sentiment analysis |
| TensorFlow / Keras  | Deep learning model                    |
| BiGRU               | Sequence classification                |
| NumPy               | Numerical computation                  |
| Pandas              | Data processing                        |
| FastAPI             | REST API development                   |
| Uvicorn             | ASGI server                            |
| HTML/CSS/JavaScript | Frontend interface                     |
| Git & GitHub        | Version control                        |
| Render              | Deployment                             |

---

## 🧠 Machine Learning Pipeline

The project follows the following NLP pipeline:

### 1. Text Collection

The model receives a textual input that needs to be classified.

### 2. Text Preprocessing

The text is cleaned and prepared for the neural network.

Typical preprocessing steps include:

* Converting text to lowercase
* Removing unnecessary characters
* Cleaning unwanted spaces
* Tokenization
* Converting text into numerical sequences
* Padding sequences to a fixed length

### 3. Text Representation

The processed text is converted into numerical representations that can be understood by the neural network.

### 4. BiGRU Model

A **Bidirectional Gated Recurrent Unit (BiGRU)** is used to understand sequential relationships in the text.

Unlike a standard GRU that processes the sequence in one direction, BiGRU processes the text in both directions:

```text
Forward  →  I really love this product
Backward ←  I really love this product
```

This allows the model to capture contextual information from both previous and following words.

### 5. Sentiment Prediction

The trained model generates a sentiment prediction based on the processed input.

---

## 📂 Project Structure

```text
Sentimental_Analysis_NLP/
│
├── Artifacts/
│   └── Trained model and preprocessing artifacts
│
├── static/
│   └── Frontend static files
│
├── final_clean.ipynb
│   └── Data preprocessing, model training and experimentation
│
├── main.py
│   └── FastAPI application
│
├── requirements.txt
│   └── Python dependencies
│
├── runtime.txt
│   └── Deployment Python runtime configuration
│
└── README.md
    └── Project documentation
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/MuskanPatel0027/Sentimental_Analysis_NLP.git
```

Navigate into the project:

```bash
cd Sentimental_Analysis_NLP
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate the environment on Windows:

```bash
venv\Scripts\activate
```

For macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the FastAPI application

```bash
uvicorn main:app --reload
```

The application will start locally.

Open:

```text
http://127.0.0.1:8000
```

---

## 🔌 API

The project uses **FastAPI** to expose the sentiment analysis functionality as a REST API.

Once the server is running, FastAPI's interactive documentation can be accessed at:

```text
http://127.0.0.1:8000/docs
```

This provides an interactive interface for testing API endpoints.

---

## 📊 Model Development

The `final_clean.ipynb` notebook contains the machine learning workflow, including:

* Data preprocessing
* Exploratory analysis
* Text preprocessing
* Tokenization
* Sequence preparation
* Deep learning model development
* BiGRU training
* Model evaluation
* Prediction experiments

---

## 🎯 Why BiGRU?

GRU networks are well suited for sequential data such as text.

A **Bidirectional GRU** provides additional contextual information by processing the sequence in both forward and backward directions.

### Advantages

* Captures long-term dependencies
* Handles sequential text efficiently
* Uses fewer parameters than many LSTM architectures
* Captures context from both directions
* Suitable for NLP classification tasks

---

## 🌐 FastAPI Integration

The trained model is integrated with FastAPI to create a lightweight prediction service.

```text
Client
  │
  │ POST text
  ▼
FastAPI
  │
  ▼
Preprocessing
  │
  ▼
BiGRU Model
  │
  ▼
Prediction
  │
  ▼
JSON Response
```

This makes the trained NLP model accessible through an API instead of limiting it to a Jupyter Notebook.

---

## ✨ Features

* ✅ NLP text preprocessing
* ✅ Deep learning-based sentiment classification
* ✅ Bidirectional GRU architecture
* ✅ FastAPI REST API
* ✅ Interactive API documentation
* ✅ Web interface
* ✅ Model artifact management
* ✅ Deployment-ready configuration

---

## 💼 Resume Description

You can describe this project on your resume as:

> **Sentiment Analysis using NLP & BiGRU** — Developed a deep learning-based sentiment classification system using NLP preprocessing and a Bidirectional GRU network. Integrated the trained model with FastAPI to provide REST-based predictions and built a web interface for user interaction.

### Technologies

**Python, NLP, TensorFlow/Keras, BiGRU, FastAPI, NumPy, Pandas, HTML, CSS, JavaScript**

---

## 👩‍💻 Author

**Muskan Patel**

* GitHub: https://github.com/MuskanPatel0027
* Repository: https://github.com/MuskanPatel0027/Sentimental_Analysis_NLP

---


If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.
