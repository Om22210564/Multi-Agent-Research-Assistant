
# 🧠 Multi-Agent Research Assistant using arXiv, RAG, Groq 

A powerful multi-agent system that helps users discover, understand, and interact with cutting-edge research papers from arXiv. The assistant supports paper search, LLM-based summarization, IEEE citation generation, and a Retrieval-Augmented Generation (RAG) pipeline to answer detailed questions about specific papers.

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![LangChain](https://img.shields.io/badge/LangChain-Enabled-yellow)
![Status](https://img.shields.io/badge/Status-Prototype-green)

---

## 📌 Features

- 🔍 **Search Papers**: Search recent papers from arXiv by topic and date range.
- 🧠 **Summarization**: Uses LLaMA 3 via Groq API to summarize each paper.
- 📄 **Citation Generator**: Formats citation in IEEE style 
- 🧾 **Interactive QA**: Ask custom questions about any paper using a RAG pipeline.
- 💾 **PDF Caching**: Avoids re-downloading papers by storing them in `/mydir`.

---

## 📂 Example Output

| Title | Summary | Citation | Paper ID |
|-------|---------|----------|----------|
| Deep Explainability in AI | A summary using ... | IEEE-style citation using Gemini... | `2305.12345` |

Users can then ask:
> “Explain the 2nd paper”  
> “What architecture is used in paper `2305.12345`?”

---

## 🔧 Tech Stack

- **[LangChain](https://www.langchain.com/)** for RAG pipeline
- **[Groq](https://console.groq.com/)** for fast LLaMA 3 summarization
- **[arXiv Python Client](https://github.com/lukasschwab/arxiv.py)** for official paper metadata and PDF access
- **FAISS + HuggingFace Embeddings** for semantic search

---

## 🚀 Getting Started

### 📦 Installation

```bash
pip install crewai langchain langchain-groq feedparser python-dotenv pandas tqdm arxiv pypdf sentence-transformers faiss-cpu

Thank you to arXiv for use of its open access interoperability.
