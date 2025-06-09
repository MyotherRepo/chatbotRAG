# 🧠 AI Lawyer - Legal Question Answering Chatbot using LangChain + Groq

This project is an **AI-powered legal assistant** built with **LangChain**, **FAISS**, and **Groq's DeepSeek LLM** to retrieve answers from legal documents. It supports PDF ingestion, vector database search, and context-aware response generation.

---

## 🚀 Features

- ✅ Uses Groq's `deepseek-r1-distill-llama-70b` model via LangChain
- 📚 Retrieves answers from a vector store of legal documents using FAISS
- 📄 Extracts context from legal documents
- 🧠 Generates context-specific answers
- ⚠️ Does **not hallucinate**—only answers based on retrieved context

---

## 🛠️ Setup Instructions
 1. Clone the Repository

```bash
git clone https://github.com/yourusername/ai-lawyer-chatbot.git
cd ai-lawyer-chatbot
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Set Up Environment Variables
Create a .env file and add your Groq API Key:

ini
Copy
Edit
GROQ_API_KEY=your_groq_api_key
4. Run the App
You can test the functionality through a script or add a frontend (e.g., Streamlit):

bash
Copy
Edit
python app.py

Project Structure
bash
Copy
Edit
.
├── app.py                 # Main chatbot script
├── vector_database.py     # FAISS vector store setup
├── .env                   # API keys (not committed)
├── requirements.txt       # Python dependencies
└── README.md              # Project overview

Example Usage
question = "If a government forbids the right to assemble peacefully which articles are violated and why?"
retrieved_docs = retrieve_docs(question)
print("AI Lawyer:", answer_query(documents=retrieved_docs, model=llm_model, query=question))

📎 Technologies Used
LangChain

Groq + DeepSeek Model

FAISS

Python-dotenv

