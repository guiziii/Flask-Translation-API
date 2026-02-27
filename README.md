# Flask Translation API

A lightweight REST API built with **Flask** that provides text translation functionality via HTTP endpoints.

Designed as a minimal microservice, this project allows applications to send text and receive translated content in response. It is simple, deployable, and easy to integrate into frontend or backend systems.

---

## 🚀 Features

- RESTful translation endpoint
- Lightweight Flask architecture
- JSON-based request/response
- Easy local setup
- Procfile support for cloud deployment
- Ready for integration with frontend or external services

---

## 📦 Requirements

- Python 3.9+
- pip

---

## 🛠 Installation

1. Clone the repository:

```bash
git clone <your-repository-url>
cd flask-main
````

2. Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # macOS/Linux
# venv\Scripts\activate    # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running Locally

```bash
python main.py
```

The API will start at:

```
http://localhost:5000
```

---

## 📡 Example Usage

### Request

```http
POST /translate
Content-Type: application/json

{
  "text": "Hello world",
  "source_language": "en",
  "target_language": "pt"
}
```

### Response

```json
{
  "translated_text": "Olá mundo"
}
```

---

## 🧪 Development Mode

```bash
export FLASK_ENV=development
export FLASK_APP=main.py
flask run
```

---

## 🌐 Deployment

This project includes a `Procfile`, allowing deployment on:

* Heroku
* Railway
* Render
* Other Procfile-compatible PaaS platforms

Example deployment:

```bash
git push heroku main
```

---

## 📁 Project Structure

```
flask-main/
│
├── main.py          # Application entry point
├── requirements.txt # Dependencies
├── Procfile         # Deployment configuration
└── .gitignore
```

---

## 🔒 Security Notes

* Store API keys using environment variables
* Do not commit secrets
* Use a production WSGI server (e.g., Gunicorn) for deployment

---

```
