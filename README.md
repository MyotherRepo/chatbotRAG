🧠 AI Lawyer - Legal Chatbot
AI-powered legal assistant that answers questions based on your uploaded legal PDFs. Built with LangChain, Groq, FAISS, and Streamlit.

🚀 Features
📄 Upload legal documents (PDFs)

🔍 Get precise legal answers based on your uploaded files

🧠 Powered by Groq LLM (deepseek-r1-distill-llama-70b)

❌ No hallucination—answers only if information is in your document

🛠️ Setup
1️⃣ Clone the repository
bash
git clone https://github.com/yourusername/ai-lawyer-chatbot.git
cd ai-lawyer-chatbot
2️⃣ Install dependencies
bash
pip install -r requirements.txt
3️⃣ Set up API key
bash
export GROQ_API_KEY=your_groq_api_key
4️⃣ Run the application
bash
streamlit run app.py
💡 Example Usage
Question: "If the government bans peaceful protest, which article is violated?"

Answer: Article 19(1)(b) guarantees the right to assemble peacefully. Banning it violates this fundamental right.
