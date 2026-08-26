# 🤖 n8n AI Automation Workflows

A collection of AI-powered automation and RAG (Retrieval-Augmented Generation) projects built using **n8n, Ollama, Qdrant, and Large Language Models (LLMs)**.

This repository contains practical AI workflow projects covering customer support, movie recommendations, and employee handbook knowledge retrieval.

---

## 🚀 Projects

### 01. Customer Support RAG

An AI-powered customer support knowledge assistant that uses RAG to retrieve relevant information from a company knowledge base and provide accurate responses.

**Key Components:**
- n8n
- RAG
- Qdrant Vector Database
- Ollama
- Embeddings
- AI Agent
- Knowledge Base

**Workflows:**
- `Knowledge_Base_Ingestion.json`
- `Knowledge_Base_Chatbot.json`

---

### 02. Movie AI Assistant

An AI-powered movie assistant that uses a movie dataset and vector search to provide movie-related recommendations and information.

**Key Components:**
- n8n
- RAG
- Qdrant
- Ollama
- Embeddings
- AI Agent
- Movie Dataset

**Workflows:**
- `Movie_Data_Ingestion.json`
- `Movie_Data_Chatbot.json`

---

### 03. Employee Handbook RAG

An AI-powered employee handbook assistant that allows users to ask questions about employee policies and retrieve relevant information from the handbook.

**Key Components:**
- n8n
- RAG
- Qdrant Vector Database
- Ollama
- Embeddings
- AI Agent
- PDF Knowledge Base

**Workflows:**
- `Employee_Handbook_Ingestion.json`
- `Employee_Handbook_Chatbot.json`

---

## 🧠 RAG Architecture

The projects follow a typical Retrieval-Augmented Generation architecture:

```text
                    DOCUMENT / DATA
                          │
                          ▼
                    Data Ingestion
                          │
                          ▼
                     Text Extraction
                          │
                          ▼
                     Text Splitting
                          │
                          ▼
                   Ollama Embeddings
                          │
                          ▼
                    Qdrant Vector DB
                          │
                          │
                    USER QUESTION
                          │
                          ▼
                       AI Agent
                          │
                          ▼
                    Query Embedding
                          │
                          ▼
                  Qdrant Retrieval
                          │
                          ▼
                       LLM
                          │
                          ▼
                    FINAL ANSWER
