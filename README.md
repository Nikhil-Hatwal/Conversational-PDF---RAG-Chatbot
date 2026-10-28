
# 🚀 Conversational PDF Chatbot

A full-stack, Dockerized **Retrieval-Augmented Generation (RAG)** system that allows users to upload PDF documents and ask questions about their contents through a conversational chatbot interface.
Built with:
- 🧠 LangChain (RAG pipeline)
- 🤖 HuggingFace Embeddings
- 🔍 FAISS Vector Store
- 🗂️ Streamlit (frontend)
- 🐳 Docker + Docker Compose

---

## 📌 Features

- Upload up to **20 PDFs**, each with **1000-page max**
- Extract, chunk, and embed documents for vector search
- Query via chatbot or REST API
- Document metadata storage using SQLite
- Dockerized for easy local or cloud deployment
- Modular architecture (Streamlit + FastAPI)

---

## 🗂️ Project Structure

```

.
├── app.py                  # Streamlit chatbot UI
├── backend/
│   ├── main.py             
├── Dockerfile              # Dockerfile for Streamlit
├── backend/Dockerfile      # Dockerfile for FastAPI
├── docker-compose.yml      # Compose setup for both services
├── requirements.txt
├── .env.example            # Example environment config
├── metadata.db             # SQLite metadata (auto-created)
├── README.md

````

## 💬 Streamlit Chat UI

* Upload PDFs
* Ask questions
* Session-aware chat
* PDF-only context enforcement

---

## 🧠 Technologies Used

| Stack       | Purpose                  |
| ----------- | ------------------------ |
| LangChain   | RAG pipeline & chains    |
| HuggingFace | Text embeddings          |
| FAISS       | Vector similarity search |
| PyPDFLoader | PDF parsing              |
| FastAPI     | REST API backend         |
| Streamlit   | Chat UI frontend         |
| SQLite      | Document metadata        |
| Docker      | Containerization         |
