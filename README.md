# RAG-based Text Retrieval System

This project implements a Retrieval-Augmented Generation (RAG) pipeline for semantic search over text data using embeddings and vector similarity search.

---

## 🔧 Features
- Sentence-based text chunking
- Embedding generation using SentenceTransformers
- Vector similarity search using FAISS
- Semantic retrieval beyond keyword matching
- Fully offline implementation (no API required)

---

## ⚙️ How it Works
1. Input text is split into manageable chunks  
2. Each chunk is converted into embeddings  
3. Embeddings are stored in a FAISS vector database  
4. User query is embedded and compared using similarity search  
5. Most relevant text chunks are retrieved and combined as the answer  

---

## 🛠️ Tech Stack
- Python  
- SentenceTransformers  
- FAISS  
- NLTK  
- NumPy  

---

## 📌 Example


**Query:**  
What does Marcus Aurelius say about controlling the mind?

**Output:**  
"He explains that one should live according to reason and not be influenced by external praise or opinions. True control lies in understanding one's inner nature and acting rationally rather than reacting to external circumstances."

## 🚀 Key Concepts
- Retrieval-Augmented Generation (RAG)  
- Embeddings  
- Vector Databases  
- Semantic Search  

---

## ⚠️ Note
This project focuses on the retrieval component of RAG. LLM-based answer generation can be added on top for more advanced responses.

---
