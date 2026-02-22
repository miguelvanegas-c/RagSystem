# 📚 RAG Example with Gemini

This project demonstrates a **Retrieval-Augmented Generation (RAG)** pipeline implemented in a Jupyter Notebook.  
It combines **document retrieval** with a **Large Language Model (LLM)** to generate more accurate, reliable, and context-aware answers.

Gemini was selected as the LLM provider due to its **generous free-tier access**, making this project fully usable without paid API credits — perfect for learning, experimentation, and academic use.

---

## 🚀 Project Overview

The notebook walks through the complete RAG workflow:

1. Load and preprocess documents  
2. Convert text into vector embeddings  
3. Store embeddings in a vector database  
4. Retrieve relevant context based on user queries  
5. Generate grounded answers using Gemini  

This approach significantly reduces hallucinations and improves factual accuracy compared to using a standalone LLM.

---

## 🏗️ Architecture & Components

The system follows a classic **RAG architecture**:

### 📄 Document Loader
- Loads and preprocesses raw text documents  
- Splits them into smaller chunks for efficient retrieval  

### 🔢 Embedding Model
- Converts text chunks into numerical vector representations  
- Embeddings are stored for similarity search  

### 🗄️ Vector Store (Retriever)
- Stores embeddings  
- Retrieves the most relevant chunks based on user queries  
- Acts as the system’s knowledge base  

### 🤖 LLM (Gemini)
- Receives the user query and retrieved context  
- Generates answers grounded in the provided documents  

### 🔁 RAG Pipeline Flow
```text
User Query → Retriever → Context → Gemini → Final Answer

