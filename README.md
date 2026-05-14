# Semantic Search Engine using Sentence Transformer 

> This project, Semantic Product Search for E-commerce using Sentence Transformers, develops an intelligent search system that improves how users find products in online shopping platforms. Traditional keyword-based search systems often fail to understand user intent and return irrelevant results when different words or synonyms are used.

To address this limitation, the system uses Sentence Transformer models to convert both user queries and product information into dense semantic embeddings. These embeddings capture the meaning of text rather than just matching keywords. Product retrieval is then performed using cosine similarity and FAISS indexing to identify and rank the most relevant products based on semantic closeness.

The system is built using a real-world e-commerce dataset and includes a full pipeline of data preprocessing, embedding generation, similarity search, and evaluation using metrics such as Precision@K and Mean Reciprocal Rank (MRR). A Streamlit-based web application is also developed to enable real-time product search with a user-friendly interface.

Overall, the project demonstrates how modern NLP techniques can significantly enhance e-commerce search systems by making them more accurate, context-aware, and user-friendly.

![License](https://img.shields.io/badge/license-Unlicense-green) ![Version](https://img.shields.io/badge/version-1.0.0-blue) ![Language](https://img.shields.io/badge/language-Python-yellow) ![GitHub](https://img.shields.io/badge/GitHub-Gyembowangs/Semantic_Search_Engine.git-black?logo=github) ![Build Status](https://img.shields.io/github/actions/workflow/status/Gyembowangs/Semantic_Search_Engine.git/ci.yml?branch=main)

## 📋 Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Tech Stack](#tech-stack)

## ℹ️ Project Information

- **👤 Author:** Gyembo Wangchuk, Sonam Dorji and Galey Mo
- **📦 Version:** 1.0.0
- **📄 License:** Unlicense
- **🌐 Website:** [https://search-engine-favwem6jgnwtsjjaumjsta.streamlit.app/](https://semanticsearchengine-ssgrroxuty7b7o8u8ad3sv.streamlit.app/)
- **📂 Repository:** [https://github.com/Gyembowangs/Semantic_Search_Engine.git](https://github.com/Gyembowangs/Semantic_Search_Engine.git)

## Features

## Features

* Semantic Search (Meaning-Based Retrieval)
- Understands user intent by matching *meaning*, not just keywords, improving relevance of search results for natural language queries.

* Sentence Transformer Embeddings
- Uses pre-trained transformer models (e.g., MiniLM, MPNet) to convert product descriptions and user queries into dense vector representations.

* FAISS Vector Search for Fast Retrieval
- Implements FAISS for efficient similarity search over large-scale embeddings, enabling fast and scalable product retrieval.


* Product Ranking using Cosine Similarity
- Ranks products based on similarity scores between query and product embeddings to ensure most relevant results appear first.

* Real-Time Search Interface (Streamlit App)
- Interactive web application where users can search products using natural language and receive instant recommendations.

* Data Preprocessing Pipeline
- Includes cleaning missing values, normalizing text, handling categorical noise, and merging product attributes into a unified search text.

* Model Evaluation and Comparison
- Evaluates multiple Sentence Transformer models using metrics like Precision@K, Recall@K, and Mean Reciprocal Rank (MRR).

* Precomputed Embeddings for Efficiency
- Stores embeddings in advance to reduce computation time and enable real-time inference during search.

* Ground Truth-Based Evaluation Setup
- Uses a semi-automated labeling approach with cross-encoder reranking to create reliable evaluation datasets.

* Product Visualization in Search Results
- Displays product image, name, price details, and relevance score in a clean grid-based UI.

* Scalable Architecture Design
-Built to handle large product datasets efficiently with modular components for preprocessing, embedding, retrieval, and deployment.


## Installation

## ⚙️ Installation Guide

### 1️. Clone the Repository

```bash
git clone https://github.com/Gyembowangs/Semantic_Search_Engine.git
cd Semantic_Search_Engine
```
### 2. Install Dependencies
```bash 
pip install -r requirements.txt
```

### 3. Verify Project Structure

### 4. Run the Application 
```bash
streamlit run app.py
```


## Tech Stack

## 🧰 Tech Stack

Python, Sentence Transformers, FAISS, BM25, Scikit-learn, Pandas, NumPy, Streamlit, Hugging Face Transformers, Pickle, Jupyter Notebook, Git & GitHub

### Core Technologies
- **NLP Models:** Sentence Transformers (MiniLM, MPNet)
- **Search Engine:** FAISS + BM25 Hybrid Retrieval
- **Backend Logic:** Python
- **Frontend:** Streamlit
- **Data Handling:** Pandas, NumPy
- **Model Storage:** Pickle

