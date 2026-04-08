# RAG Math PDF Assistant

A Retrieval-Augmented Generation (RAG) system that answers mathematical questions using content from PDF documents. The system retrieves relevant document sections using vector similarity search and generates structured answers using a language model.

## Overview
This project implements a semantic question-answering system for mathematical documents. Instead of relying solely on a language model, the system retrieves relevant passages from uploaded PDFs and uses them as context for generating accurate answers.

The system was designed to work with technical mathematical content, including symbolic expressions and LaTeX formatting.

## Features
- Upload and process mathematical PDF documents
- Automatic document chunking and embedding generation
- Vector similarity search using FAISS
- Retrieval-Augmented Generation (RAG) pipeline
- Structured responses with LaTeX-style mathematical formatting
- Context-aware answer generation using an LLM
- Interactive UI built with Gradio
- LaTeX-formatted math responses 

## Technologies Used
- Python
- FAISS (vector similarity search)
- Hugging Face Transformers
- Phi-3-mini language model
- Gradio (interactive UI)

## How It Works
1. PDFs are parsed and split into smaller text chunks.
2. Each chunk is converted into vector embeddings.
3. Embeddings are stored in a FAISS index for fast similarity search.
4. When a user asks a question, the system retrieves the most relevant document chunks.
5. The retrieved context is passed to the language model to generate an answer.

## Example Use Case
Ask: "What is eigenvalue decomposition?"
The model then retrives relevant sections from the PDF and generates a structured explanation with math formatting

## Future Improvements
- Support for multiple PDF documents
- Improved mathematical symbol parsing
- Enhanced retrieval ranking
- Web-based interface deployment
