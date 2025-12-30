# 🌍 Multilingual AI Summarizer

This project is a **multilingual text summarizer** built with **FastAPI (backend)** and **Gradio (frontend)**.  
It supports summarization of **English, Telugu, Hindi, Pashto, and other languages** using the `csebuetnlp/mT5_multilingual_XLSum` model from HuggingFace.

---

## 🚀 Features
- Upload **PDF, DOCX, TXT** files or paste text.
- Automatic **language detection** with `langid`.
- Summarization powered by **mT5 XLSum**.
- Backend: **FastAPI** REST API.
- Frontend: **Gradio UI** for easy use.
- Ready for deployment on **Heroku** or **Render**.

---

## 🛠️ Installation (Local Setup)

1. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/multilingual-summarizer.git
   cd multilingual-summarizer

▶️ Running Locally
1. Start Backend (FastAPI)
uvicorn backend:app --reload


👉 Runs on: http://127.0.0.1:8000
👉 API docs: http://127.0.0.1:8000/docs

2. Start Frontend (Gradio)
python frontend.py


👉 Runs on: http://127.0.0.1:7860

🌐 Deployment
Heroku

Install Heroku CLI

Login:

heroku login


Create app:

heroku create my-ai-summarizer


Deploy:

git push heroku main


Your backend will be live at:

https://my-ai-summarizer.herokuapp.com/summarize


Update frontend.py with this URL:

API_URL = "https://my-ai-summarizer.herokuapp.com/summarize"


Run frontend locally → it will call your cloud API.

📖 API Usage

Endpoint: POST /summarize
Parameters:

text: Input text (string, optional)

file: Upload file (.pdf, .docx, .txt)

max_length: (default 150)

min_length: (default 40)

Example (cURL):

curl -X POST "http://127.0.0.1:8000/summarize" \
  -F "text=William Shakespeare is one of the greatest writers..."

📷 Screenshots

(Add screenshots of your Gradio UI and FastAPI docs here)

📝 Future Improvements

Support for more file formats (Excel, HTML).

GPU acceleration (Torch with CUDA).

Deploy frontend and backend together.

👨‍💻 Author

Your Name – Nekkanti Satya Srinath 


---

👉 This way your `README.md` explains everything from **setup → usage → deployment**.  

Do you want me to also create a **short version** (like one-page quick-start only) for GitHub, and keep this **long version in a separate docs/ folder**?
