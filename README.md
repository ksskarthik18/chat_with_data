📄 Chat with Your Data – RAG-Based PDF Question Answering System

🚀 Overview
Chat with Your Data is a Retrieval-Augmented Generation (RAG) application that enables users to upload PDF documents and ask questions in natural language. The system retrieves relevant document sections using vector search and generates context-aware answers using LLaMA 3 powered by Groq.

✨ Features
- PDF document ingestion and processing
- Automatic text chunking with overlap
- Vector-based semantic retrieval using FAISS
- Context-aware question answering
- Source-based response generation
- Fast inference using Groq LLaMA 3

🏗️ Architecture

```text
PDF
 ↓
Text Extraction
 ↓
Chunking
 ↓
Embeddings
 ↓
FAISS Vector Database
 ↓
Similarity Search
 ↓
Groq LLaMA 3
 ↓
Answer Generation
```

🛠️ Tech Stack

Programming Language
- Python

LLM
- LLaMA 3 (Groq API)

Vector Database
- FAISS

Libraries
- LangChain Community
- PyPDF
- Python Dotenv

Concepts Used
- Retrieval-Augmented Generation (RAG)
- Semantic Search
- Vector Embeddings
- Similarity Search
- Prompt Engineering
- Text Chunking

📂 Project Structure

```text
chat-with-your-data/
│
├── rag_chat.py
├── .env
├── requirements.txt
└── README.md
```

⚙️ Installation

Clone Repository

```bash
git clone <repository-url>
cd chat-with-your-data
```

Install Dependencies

```bash
pip install -r requirements.txt
```

Configure API Key

Create a `.env` file:

```env
GROQ_API_KEY=your_api_key_here
```

▶️ Run the Project

```bash
python rag_chat.py
```

🧪 Sample Questions

- What are the classification categories used in NIDS?
- How does STL perform compared to SMR?
- What are the advantages of cloud-based IDS?
- Explain the role of ROC curves in intrusion detection.

📈 Future Enhancements

- Multi-PDF support
- Web interface using Streamlit
- Persistent FAISS storage
- Source highlighting
- Chat history memory
- API deployment using FastAPI
