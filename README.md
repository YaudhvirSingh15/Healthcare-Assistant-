# Healthcare-Assistant-
# 🩺 AI Healthcare Assistant (RAG-Powered)

An intelligent clinical decision support and patient Q&A assistant powered by **Retrieval-Augmented Generation (RAG)**. This system retrieves verified clinical guidelines, medical textbooks, and research papers to generate grounded, context-aware answers.

> ⚠️ **Medical Disclaimer:** This system is for informational and research purposes only. It does not provide medical diagnoses or replace professional clinical judgment.

---

## 🌐 Architecture Overview

1. **Document Ingestion:** Parses medical PDFs and clinical guidelines.
2. **Chunking & Vectorization:** Text is chunked and embedded using specialized embeddings.
3. **Vector Storage:** Embedded vectors are stored in a vector database for semantic similarity search.
4. **Contextual Retrieval:** Retrieves top $k$ relevant passages based on user queries.
5. **Grounded Generation:** An LLM generates responses using only retrieved medical context with safety guardrails.

---

## 📁 Repository Structure

- `src/data_ingestion.py`: Loads and cleans clinical documents.
- `src/vector_store.py`: Handles vector indexing and vector DB management.
- `src/rag_chain.py`: Configures the prompt template, context retrieval, and LLM output pipeline.
- `src/app.py`: Frontend interface built with Streamlit.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- OpenAI API Key (or local LLM environment setup)

### Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/ai-healthcare-assistant-rag.git](https://github.com/your-username/ai-healthcare-assistant-rag.git)
   cd ai-healthcare-assistant-rag
