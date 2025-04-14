# Simple Local RAG Tutorial

This project demonstrates how to build a **Retrieval Augmented Generation (RAG)** pipeline locally to query documents (e.g., a PDF nutrition textbook) and generate responses using a **Large Language Model (LLM)**. The pipeline retrieves relevant information from document chunks and generates answers based on those passages, all running locally on your own hardware.

## Overview

The **NutriChat** pipeline allows you to interact with a **1200-page PDF nutrition textbook**. By querying this document, the pipeline uses an LLM to generate responses based on relevant passages of the text. This process runs locally on your hardware, with support for NVIDIA GPUs for faster computation.

The system utilizes the following components:
- **Document Preprocessing**: Splits the document into smaller chunks.
- **Embedding Generation**: Converts queries into vector embeddings.
- **Retrieval**: Finds relevant document chunks based on the query embedding.
- **Generation**: Uses an LLM to generate a response based on the retrieved passages.

## Features

- **Local Execution**: Run everything on your own machine without relying on external APIs.
- **Fast Querying**: Retrieve information quickly using an efficient retrieval method.
- **LLM-Based Generation**: Get human-like responses from a pre-trained LLM.
- **PDF Support**: The pipeline works specifically with PDF documents, like textbooks.

## Prerequisites

- **Python 3.11+**
- **NVIDIA GPU** (for faster inference, minimum 5GB VRAM recommended)
- Basic knowledge of **Python**, **PyTorch**, and **Natural Language Processing (NLP)**.
- **Jupyter Notebook** or **VS Code** for running the code.

## RAG (Retrieval Augmented Generation)

RAG combines **retrieval** and **generation**:

- **Retrieval**: Fetches relevant information from a document or database.
- **Generation**: Generates answers using a pre-trained language model, grounded in the retrieved data.

This allows the system to answer queries by retrieving knowledge from a document and generating responses based on that context.

## Why Run Locally?

Running the RAG pipeline locally offers several advantages:
- **Privacy**: Your data stays on your own machine, ensuring privacy.
- **Cost-Effective**: No ongoing costs like API charges.
- **Customization**: You can easily modify the pipeline to fit your needs.

## Key Concepts

| **Term**                  | **Description** |
|---------------------------|-----------------|
| **Token**                  | Sub-word unit of text. |
| **Embedding**              | A vector representation of text. |
| **Embedding Model**        | A model that generates embeddings for input data. |
| **Similarity Search**      | Searching for similar embeddings using cosine similarity. |
| **LLM (Large Language Model)** | A model trained to generate human-like text. |
| **Context Window**         | The number of tokens the LLM can process at once. |
| **Prompt**                 | The text input to an LLM for generating output. |

## Usage

Once the setup is complete, you can query the document via the notebook interface. For example, you could ask questions like:
- "What are the benefits of carbohydrates?"
- "Explain the role of vitamins in human health."

The system will retrieve relevant passages and generate answers based on the context.

## Extensions

### Future Features:
- Integration with more document sources, such as websites and databases.
- Improvements in the retrieval and generation mechanisms for faster and more accurate responses.
