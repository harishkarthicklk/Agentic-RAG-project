# Agentic RAG System for YouTube Knowledge Bases

## Overview

This project implements an Agentic Retrieval-Augmented Generation (RAG) system that converts YouTube videos into a searchable knowledge base. The system uses Whisper for transcription, MongoDB Atlas Vector Search for semantic retrieval, and local LLMs (Llama 3/Mistral) for answer generation.

A LangGraph-based routing mechanism dynamically decides whether a query should be answered using retrieved knowledge or by a direct LLM response.

---

## Features

- YouTube video ingestion
- Speech-to-text transcription using Whisper
- Document preprocessing and chunking
- Embedding generation using HuggingFace models
- MongoDB Atlas Vector Search
- Agentic routing with LangGraph
- Local LLM integration (Llama 3 / Mistral)
- LangSmith evaluation with LLM-as-a-Judge

---

## Architecture

![Architecture](architecture.png)

---

## Workflow

1. Collect YouTube videos
2. Convert audio to text using Whisper
3. Create structured documents
4. Split documents into chunks
5. Generate vector embeddings
6. Store embeddings in MongoDB Atlas
7. Perform semantic retrieval using Vector Search
8. Route queries using LangGraph
9. Generate responses using RAG or Direct LLM
10. Evaluate performance using LangSmith

---

## Tech Stack

- Python
- LangChain
- LangGraph
- MongoDB Atlas
- Whisper
- HuggingFace Embeddings (BAAI/bge-small-en-v1.5)
- Ollama
- Llama 3
- Mistral
- LangSmith

---

## Evaluation Results

### Routing Evaluation

- Routing Accuracy: **87.5%**

### Answer Quality Evaluation (LLM-as-a-Judge)

- Correctness: **0.75**
- Relevance: **0.77**
- Helpfulness: **0.79**


---

## Future Improvements

- Streamlit/Web UI
- Conversation memory
- Hybrid search (keyword + vector)
- Reranking
- Advanced RAG evaluation metrics

---

## Author

Harish Karthick L K

Integrated M.Tech Student | AI/ML Enthusiast