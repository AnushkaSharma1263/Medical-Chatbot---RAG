🏥 AI Medical Bot using RAG (Retrieval-Augmented Generation)
An intelligent medical chatbot powered by Retrieval-Augmented Generation (RAG) architecture, designed to provide accurate, context-aware, and trustworthy medical information by combining Large Language Models (LLMs) with a vector database for domain-specific retrieval.

📌 Project Overview
This AI Medical Bot answers health-related queries by retrieving relevant medical knowledge from trusted sources before generating responses.
Unlike vanilla LLMs, which rely solely on pre-trained data, this bot uses RAG to:

Search a curated medical knowledge base.

Retrieve the most relevant documents.

Generate concise, medically-informed answers.

⚠ Disclaimer: This bot is for educational and informational purposes only and should not replace professional medical advice.

🛠️ Tech Stack
Programming Language: Python

Framework: LangChain

LLM API: OpenAI GPT / Groq LLM

Vector Database: FAISS

Frontend: Streamlit

Other Tools: HuggingFace Transformers, Sentence Transformers for embeddings

📂 Project Architecture
flowchart TD
    A[User Query] --> B[Embed Query]
    B --> C[Search in Vector DB]
    C --> D[Retrieve Relevant Medical Docs]
    D --> E[Pass Docs + Query to LLM]
    E --> F[Generate Answer]
    F --> G[Display Response to User]


✨ Features
Medical Knowledge Base – Curated from reliable sources like WHO, NIH, and research papers.

RAG Workflow – Ensures context-aware answers with supporting evidence.

Multi-turn Conversations – Maintains chat history for better context.

Fast Retrieval – Optimized embeddings & vector search.

User-Friendly UI – Streamlit-powered web interface.

🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/AnushkaSharma1263/Medical-Chatbot-RAG.git
cd Medical-Chatbot-RAG

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Set Environment Variables
Create a .env file:

OPENAI_API_KEY=your_openai_api_key
GROQ_API_KEY=your_groq_api_key

4️⃣ Run the Application
streamlit run app.py

📊 Example Queries
"Explain symptoms of diabetes."
"Suggest preventive measures for high blood pressure."
"What are the common side effects of Ibuprofen?"

🧩 Folder Structure
ai-medical-bot-rag/
│-- data/                # Medical documents / datasets
│-- embeddings/          # Precomputed embeddings
│-- app.py                # Streamlit frontend
│-- rag_pipeline.py       # RAG implementation
│-- requirements.txt      # Python dependencies
│-- README.md             # Project documentation


🔮 Future Enhancements
✅ Voice input/output integration

✅ Multi-language medical support

✅ HIPAA-compliant data handling for real-world deployment

🛡 Disclaimer
This bot does not provide medical diagnosis or treatment. Always consult a licensed healthcare provider for medical concerns.

🤝 Contributing
Contributions are welcome!

Fork this repository

Create your feature branch (git checkout -b feature/xyz)

Commit changes (git commit -m 'Add xyz feature')

Push to branch (git push origin feature/xyz)

Open a Pull Request

