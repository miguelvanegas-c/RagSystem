# RAG Example with Gemini

This project demonstrates a Retrieval-Augmented Generation (RAG) pipeline implemented in a Jupyter Notebook.
The notebook shows how to combine document retrieval with a Large Language Model (LLM) to generate more accurate and context-aware answers.

I selected Gemini as the LLM provider because it offers the most generous free-tier access, making this project accessible without requiring paid API credits.

# Project Architecture and Components

The system follows a classic RAG architecture:

Document Loader

- Loads and preprocesses text documents.

- Splits them into smaller chunks for efficient retrieval.

Embedding Model

- Converts text chunks into numerical vector representations.

- These embeddings are stored in a vector database for similarity search.

Vector Store (Retriever)

- Stores embeddings and retrieves the most relevant chunks given a user query.

- Acts as the “knowledge base” of the system.

LLM (Gemini)

- Receives both the user question and the retrieved context.

- Generates a final answer grounded in the retrieved documents.

RAG Pipeline

- User Query → Retriever → Context → Gemini → Final Answer

This approach reduces hallucinations and improves factual accuracy compared to using an LLM alone.


# How to Run the Notebook

- Start Jupyter Notebook:

jupyter notebook

- Open:

RAGExample.ipynb

- Run all cells step by step:

Load documents

Generate embeddings

Store them in the vector database

Ask questions and receive answers from Gemini using retrieved context



# Why Gemini?

- Free-tier access with generous limits

- Strong performance for question answering

- Easy integration with Python

- Ideal for academic and experimental projects

This makes Gemini an excellent choice for building RAG systems without financial barriers.

