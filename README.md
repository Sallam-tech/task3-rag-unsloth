# Task 3 — Retrieval Augmented Generation (RAG) with Unsloth

This repository contains **Task 3** of the Generative AI internship:  
a clean implementation of **Retrieval Augmented Generation (RAG)** using an **Unsloth dynamic 4-bit language model** on Google Colab.

---

## 🚀 Overview

The notebook implements a complete end-to-end RAG pipeline that:

- Loads a **4-bit quantized LLM** using **Unsloth**
- Generates embeddings using **sentence-transformers (CPU)**
- Indexes documents using **FAISS**
- Retrieves relevant documents for a user query
- Generates **grounded answers strictly from retrieved context**

---

## 🧠 Architecture

**Generator (LLM)**
- Model: Mistral-7B-Instruct
- Quantization: Dynamic 4-bit (Unsloth)
- Hardware: GPU (T4)

**Retriever**
- Embedding model: `all-MiniLM-L6-v2`
- Vector store: FAISS (`IndexFlatL2`)

**Knowledge Source**
- Simple plain-text documents
- No PDFs or external scraping

---

## 📁 Files

- Fully runnable from top to bottom
- Clean and minimal notebook
- Designed for evaluation and submission

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**
2. Enable **GPU (T4)**
3. Run all cells sequentially from top to bottom

---

## ✅ Requirements Covered

- Unsloth dynamic 4-bit model  
- CPU-based embeddings  
- FAISS-based retrieval  
- Context-grounded answer generation  
- Clean, minimal RAG implementation  

---

## 📌 Notes

- This task focuses **only on RAG**
- Speech or audio components are intentionally excluded
- The implementation avoids unnecessary dependencies and complexity



