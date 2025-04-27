
# AICHATBOT USING PYTHON

## 🔍 Overview

**AICHATBOT USING PYTHON** is an intelligent, intent-based chatbot built using Natural Language Processing (NLP) techniques and Deep Learning. It is capable of understanding user intents, responding accordingly, and even integrating external APIs to provide real-time information. This chatbot can be deployed in various industries for customer support, query handling, or general conversation.

The system is built with Python, using the **NLTK** library for preprocessing and **PyTorch** to train a **Feedforward Neural Network (FNN)** model. It also integrates **Flask** to build an API and features a responsive **ReactJS** frontend for an engaging user experience.

---

## ⚙️ Key Features

- **Intent Recognition** using NLP.
- **Bag of Words**, **Tokenization**, and **Stemming** with NLTK.
- **Deep Learning Model** using PyTorch.
- **API Integrations**:
  - Weather (OpenWeatherMap)
  - Movies (TheMovieDB)
  - Wikipedia (Factual information lookup)
- **Flask Backend** for API endpoints.
- **ReactJS Frontend** for an interactive user interface.
- **Customizable** intents and responses for different use cases.
- **Cloud Deployment Ready** (e.g., Render).

---

## 🧠 How it Works

### 1. Data Preparation

The chatbot uses a JSON-based `intents.json` file, which maps user input patterns to specific intents and provides possible responses.

### 2. Data Preprocessing

- Tokenization
- Stemming
- Bag of Words conversion

### 3. Model Training

- Feedforward Neural Network using PyTorch.
- Trained on preprocessed intent data.
- Saved for real-time predictions.

### 4. Chat Interface and Response

- User input is classified into intents.
- Specific response or API call is triggered based on the intent.

---

## 📦 Folder Structure

```
AI-Chatbot-DL-NLP/
├── chatbotui/               # ReactJS frontend
├── intents.json             # Intent data
├── nltk_utils.py            # Tokenization and BoW utilities
├── model.py                 # Neural network class
├── train.py                 # Training script
├── chat.py                  # Chat handler using trained model
├── app.py                   # Flask backend for API endpoint
├── requirements.txt         # Python dependencies
└── README.md                # This file
```

---

## 🚀 Getting Started

### 1. Clone the Repository & Set Up Environment
```bash
git clone https://github.com/yourusername/AI-Chatbot-DL-NLP.git
cd AI-Chatbot-DL-NLP
python -m venv venv
venv\Scripts\activate  # For Windows
```

### 2. Install Dependencies
```bash
(venv) pip install -r requirements.txt
```

### 3. Install NLTK Data
```bash
(venv) python
>>> import nltk
>>> nltk.download('punkt')
>>> exit()
```

### 4. Train the Model
```bash
(venv) python train.py
```

### 5. Start Chatting (Local Testing)
```bash
(venv) python chat.py
```

---

## 🌐 API Integration (Optional)

To enable **Weather** or **Movie** responses:

- Get API keys from:
  - [OpenWeatherMap](https://openweathermap.org/api)
  - [TheMovieDB](https://developer.themoviedb.org)

- Add logic in `chat.py`

- Install requests module if not available:
```bash
pip install requests
```

---

## 🌍 Deploying Backend API (Flask)

Run Flask endpoint locally:

```bash
(venv) python app.py
```

Deploy the backend on cloud (e.g., Render).

---

## 💬 Frontend UI with React

Inside the `chatbotui/` folder:

```bash
npm install
npm start
```

---

## 🎯 Use Cases

- E-commerce Customer Support
- Healthcare Assistants
- FAQ Bots
- Educational Help Desks

---

## 📚 References

- [NLTK Documentation](https://www.nltk.org/)
- [PyTorch Documentation](https://pytorch.org/)
- [OpenWeatherMap API](https://openweathermap.org/api)
- [TheMovieDB API](https://developer.themoviedb.org)
- [Wikipedia Library](https://pypi.org/project/wikipedia/)

---

## 📄 License

This project is licensed under the MIT License.
