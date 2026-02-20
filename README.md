# 🧠 Semantic Search Engine for E-commerce (SBERT + FAISS)

An end-to-end semantic product search system built in Google Colab using NLP and vector similarity search.

This project shows how product descriptions can be transformed into semantic embeddings to retrieve relevant items based on meaning rather than keywords.


## 🚀 Project Highlights

- Semantic embeddings with Sentence-BERT

- Fast similarity search using FAISS

- Evaluation using Precision@k, Recall@k, MRR

- Embedding visualization with UMAP

- Implemented and tested in Google Colab

## 📦 Dataset

This project uses the **Flipkart Fashion Products Dataset** from Kaggle:  
https://www.kaggle.com/datasets/aaditshukla/flipkart-fasion-products-dataset/data  

The dataset contains e-commerce product information such as **title, description, brand, category, and sub-category**.  
These textual fields are combined and processed to generate **semantic embeddings** that power the similarity search system.

## 📓 Open in Google Colab

Run the notebook directly: https://colab.research.google.com/drive/15ePQAyXHorcihkKymnigCeyJBZRU1WrP?authuser=1

## 🧩 Workflow Overview

### Data Cleaning & Preprocessing

- Combine product text fields (title, description, brand, category)

- Normalize and clean text

### Generate Embeddings

- Use SBERT (all-MiniLM-L6-v2) to encode products into 384-dimensional vectors

### Build Vector Index

- Store embeddings in a FAISS index for fast similarity search

### Semantic Search

- Convert user query into embedding

- Retrieve top-k similar products

### Visualization

- UMAP projection of embeddings to explore product clusters

## 🛠️ Technologies Used

- Python

- Pandas / NumPy

- Sentence-Transformers (SBERT)

- FAISS

- UMAP

- Matplotlib / Seaborn

- Google Colab

## ▶️ How to Run

- Open the notebook in Google Colab

- Run all cells step by step:

- Install dependencies

- Load dataset

- Generate embeddings

- Build FAISS index

- Run search queries

- Visualize embeddings

## 📊 Example Query

Input: "black shirt for men" 

The system retrieves products based on semantic similarity, not exact keyword matches.

## 🔮 Future Improvements

- Better dataset with category balance

- User interface

## 👤 Author

Romain Reina