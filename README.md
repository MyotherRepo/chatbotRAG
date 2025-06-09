# 🧠 AI Lawyer - Legal Question Answering Chatbot using LangChain + Groq

This project is an **AI-powered legal assistant** built with **LangChain**, **FAISS**, and **Groq's DeepSeek LLM**. It retrieves context from uploaded legal PDFs and answers questions based strictly on that context. Designed to **not hallucinate**, it only answers when the information exists in the uploaded documents.

---

## 🚀 Features

- ✅ Uses Groq’s `deepseek-r1-distill-llama-70b` LLM
- 📄 Accepts legal PDFs from users
- 🧠 Answers questions strictly using document context
- ❌ Avoids hallucination and fabricating answers
- 🔍 Vector-based similarity search via FAISS
- 🌐 Simple UI using Streamlit

---

## 📦 Folder Structure

.
├── app.py # Streamlit app combining upload, vector DB, and LLM
├── README.md # This documentation
├── requirements.txt # Required Python packages
├── .env # Groq API key (not included in repo)


---

## ⚙️ Setup Instructions

1. Clone the Repository
    ```bash
   git clone https://github.com/yourusername/ai-lawyer-chatbot.git
   cd ai-lawyer-chatbot
2. Create and Activate a Virtual Environment (Optional)
        python -m venv venv
     source venv/bin/activate       # macOS/Linux
     venv\Scripts\activate          # Windows

3. Install Requirements
    pip install -r requirements.txt 
4. Add .env File
    GROQ_API_KEY=your_groq_api_key

🧪 How It Works
Upload a legal PDF

App splits and embeds the content using HuggingFace embeddings

FAISS vector store performs similarity search for each query

Groq LLM answers strictly from relevant document chunks

🧠 Example Question
question = "If a government forbids the right to assemble peacefully, which articles are violated and why?"
AI Lawyer: According to Article 19(1)(b) of the Constitution, all citizens shall have the right to assemble peaceably and without arms. Violating this constitutes a breach of fundamental rights.

