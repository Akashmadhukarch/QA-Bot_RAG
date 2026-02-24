# 🧠 RAG-Based Customer Support QA Chatbot

This project implements a Retrieval-Augmented Generation (RAG) based Question Answering Chatbot using:

- 🔍 Selenium Web Scraping
- ✂ Recursive Text Splitting
- 🧠 HuggingFace Embeddings
- 🗂 Deep Lake Vector Database
- 🚀 Groq LLM (LLaMA 3.1)
- 🧩 LangChain Framework

The chatbot answers questions strictly based on provided website content, reducing hallucinations and improving factual grounding.

---

## 📌 Project Architecture
Website URLs
↓
Selenium Scraping
↓
Text Cleaning
↓
Recursive Text Splitter (500 chunk / 100 overlap)
↓
HuggingFace Embeddings (all-mpnet-base-v2)
↓
Deep Lake Vector Store
↓
Retriever (Top-K Similarity Search)
↓
Groq LLM (llama-3.1-8b-instant)
↓
Final Grounded Answer
                                                    * working*  
 - Scrapes real website content
- Converts content into vector embeddings
- Stores embeddings in Deep Lake
- Retrieves only relevant chunks
- Uses strict prompt to prevent hallucination
- Answers only from provided knowledge base
!!!!!setup   
pip install langchain==0.1.17
pip install langchain-community==0.0.35
pip install langchain-core==0.1.52
pip install langchain-groq==0.1.4
pip install deeplake
pip install sentence-transformers
pip install selenium
pip install webdriver-manager
pip install unstructured
pip install notebook
