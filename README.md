# 📄 RAG-Based Question Answering System (FAISS + SentenceTransformers)

## 🚀 Overview
This project implements a **Retrieval-Augmented Generation (RAG)** pipeline to answer questions from a text document (*Meditations by Marcus Aurelius*).

The system performs **semantic search using FAISS** to retrieve the most relevant text chunks and returns a clean, context-based answer.  
A lightweight LLM integration was explored for answer generation.

---

## 🧠 How It Works

1. **Text Processing**
   - Load raw text file
   - Split into meaningful chunks using sentence-based chunking (NLTK)

2. **Embeddings**
   - Convert text chunks into vector representations using `SentenceTransformers`

3. **Vector Database**
   - Store embeddings in **FAISS** for efficient similarity search

4. **Retrieval**
   - Given a query, retrieve top-k relevant chunks using semantic similarity

5. **Answer Generation**
   - Return the most relevant cleaned text as the final answer  
   - Use a lightweight LLM for response generation

---

## 🛠️ Tech Stack

- Python  
- SentenceTransformers  
- FAISS  
- LangChain (retriever usage)  
- NLTK (text chunking)  
- HuggingFace Transformers (optional LLM)

---

## 📌 Example

**Query:**  
What does Marcus Aurelius say about controlling the mind?

**Output:**  
He explains that one should live according to reason and not be influenced by external praise or events. Control comes from within, and one must act according to nature.

---

## ⚠️ Note

- This project focuses on **retrieval quality**, which is the core of RAG systems.
- A lightweight LLM was tested, but due to limitations, final answers are primarily retrieval-based.
- Stronger instruction-tuned models can significantly improve answer generation.

---
## 🎯 Key Learnings

- Built an end-to-end **RAG pipeline**
- Understood **vector databases (FAISS)** and similarity search
- Implemented **text chunking and embedding pipelines**
- Integrated retrieval with basic LLM experimentation
- Handled real-world issues like noisy text cleaning

---

## 📌 Future Improvements

- Use stronger LLMs (e.g., GPT, LLaMA) for better answers  
- Add FastAPI for deployment  
- Build a UI for user interaction  

---
