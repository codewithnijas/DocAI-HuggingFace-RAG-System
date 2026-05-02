📄 DocAI — AI PDF Chatbot (RAG with HuggingFace + FAISS)

An intelligent PDF Question Answering system built using Retrieval-Augmented Generation (RAG).
Upload any PDF and ask natural language questions — powered by HuggingFace LLMs + semantic search.

🚀 Live Features
📄 Upload and analyze any PDF
🧠 AI-powered question answering (RAG pipeline)
🔍 Semantic search using FAISS vector database
🤖 HuggingFace LLM (Qwen2.5 / other models)
📚 Source-aware answers (page references)
💬 Interactive Gradio chat UI
⚡ Fast embedding with SentenceTransformers
🧠 Architecture Overview
🖼️ System Workflow
📄 PDF → ✂️ Chunking → 🔢 Embeddings → 🧠 FAISS Index
                                          ↓
💬 User Question → 🔍 Similarity Search → 🤖 LLM → 📢 Answer
📸 Screenshots
🖥️ Main Interface

![UI Screenshot](assets/ui.png)
⚙️ Tech Stack
LangChain – RAG pipeline orchestration
FAISS – Vector similarity search
SentenceTransformers – Embeddings model
HuggingFace Inference API – LLM (Qwen2.5)
PyPDF – PDF parsing
Gradio – Web UI
📦 Installation
git clone https://github.com/your-username/DocAI.git
cd DocAI

pip install -r requirements.txt
🔐 HuggingFace Setup

Create a token here: https://huggingface.co/settings/tokens

Then set it in environment:

import os
os.environ["HUGGINGFACEHUB_API_TOKEN"] = "your_token_here"
🚀 Run the Project
Option 1: Jupyter / Colab

Run DocAI.ipynb step by step.

Option 2: Gradio App
python app.py
🧪 Example Questions
What is this document about?
Summarize key points
What are the conclusions?
Explain section 3 in simple terms
🧱 Project Structure
DocAI/
│
├── DocAI.ipynb
├── app.py
├── requirements.txt
├── README.md
└── assets/
    ├── ui.png
    ├── chat.png
    └── process.png
🧠 How It Works (RAG Pipeline)
PDF is loaded using PyPDFLoader
Text is split into chunks
Each chunk is converted into embeddings
Stored in FAISS vector database
User question is embedded
Similar chunks are retrieved
Context is sent to LLM (Qwen2.5)
Final grounded answer is generated
📌 Future Improvements
🔥 Streaming responses
🧠 Memory-based chat history
🌐 Deploy on HuggingFace Spaces
📊 PDF highlighting in UI
🧾 Multi-document Q&A
👨‍💻 Author

Muhammed Nijas

⭐ If you like this project

Give it a ⭐ on GitHub and share it!
