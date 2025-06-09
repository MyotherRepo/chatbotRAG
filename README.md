# 🧠 AI Lawyer - Legal Chatbot using LangChain + Groq

This is an **AI-powered legal assistant** that answers questions based on your uploaded legal PDFs. Built with **LangChain**, **Groq**, **FAISS**, and **Streamlit**.

---

## 🚀 Features

- 📄 Upload legal PDFs
- 🧠 Asks legal questions based on your documents
- ✅ Groq LLM (`deepseek-r1-distill-llama-70b`)
- ❌ No hallucination — answers only if info is in your doc

---

## 🛠️ Setup

### 1. Clone this repo

```bash
git clone https://github.com/yourusername/ai-lawyer-chatbot.git
cd ai-lawyer-chatbot
pip install -r requirements.txt
GROQ_API_KEY=your_groq_api_key
streamlit run app.py

💡 Example Use
Question: "If the government bans peaceful protest, which article is violated?"
Answer: "Article 19(1)(b) guarantees the right to assemble peacefully. Banning it violates this fundamental right."
