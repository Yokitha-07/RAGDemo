## RAG with LangChain, FAISS, and Hugging Face
Overview

This project implements a Retrieval-Augmented Generation (RAG) pipeline using:

LangChain for building the RAG chain

FAISS to store and retrieve document embeddings

Sentence Transformers to convert text into embeddings

Hugging Face LLM (Qwen) to generate answers from retrieved context

The system answers questions using only the content of a provided text file.

## Features

Load a text document (About_Ai.txt)

Split it into small chunks for better retrieval

Convert chunks into embeddings with sentence-transformers

Store embeddings in FAISS for fast similarity search

Retrieve relevant chunks for a question

Generate answers using a Qwen text-generation model

Handles “I don’t know” if the answer is not in the context
