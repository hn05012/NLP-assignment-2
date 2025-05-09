# NLP-assignment-2

# Document Retriever with FAISS and SentenceTransformers

## Overview

This project implements a **Retriever** class designed to handle document indexing and search using **FAISS** (Facebook AI Similarity Search) and **SentenceTransformers**. The class supports adding documents, querying them, and saving/loading the index. It processes text documents and chunks them to improve search accuracy and efficiency.

## Features
- **Chunking and Indexing**: The retriever handles the chunking and indexing of documents internally.
- **Real Document Support**: The retriever supports `.txt`, `.md`, and `.pdf` files. You can preprocess and chunk these files for indexing.
- **Search and Query**: You can query documents based on their contents and retrieve the most relevant chunks.
- **FAISS and SentenceTransformers**: Uses FAISS for efficient similarity search and SentenceTransformers for transforming documents into vector embeddings.

## Methods

### 1. `add_documents(documents)`
Adds documents to the retriever for indexing.

### 2. `query(query_string, top_k=1)`
Queries the indexed documents and returns the top `k` most relevant chunks for the provided query.

### 3. `save(file_path)`
Saves the indexed documents to a file for later use.

### 4. `load(file_path)`
Loads previously saved indexed documents from a file.

## Installation

To install the necessary dependencies, run the following:

```bash
pip install faiss-cpu sentence-transformers


## Usage

## Step by Step Guide

### 1. Import the Retriever class:


```{python}
from retriever import Retriever
```
