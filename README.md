# Generative AI in Finance: Introduction to LLMs and RAG

This repository contains a Jupyter notebook that demonstrates how to build a financial Question-Answering system using Generative AI, specifically Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG).

## Overview

The notebook walks through the following steps:
1.  **Setup**: Installing necessary Python libraries like `openai`, `pinecone-client`, `chromadb`, `langchain`, and `pandas`.
2.  **Data Loading and Chunking**: Loading a sample financial policy CSV and splitting it into manageable chunks.
3.  **Vector Embeddings**: Creating vector embeddings of the text chunks using OpenAI's models.
4.  **Vector Stores**: Storing and indexing the embeddings in both ChromaDB (for local, open-source use) and Pinecone (for a scalable, cloud-based solution).
5.  **RAG Implementation**: Building a retrieval-based QA chain using LangChain to answer questions based on the financial document.
6.  **Example Q&A**: Demonstrating how to ask questions and get context-aware answers from the system.

## Key Technologies

*   **Python**: The primary programming language.
*   **Jupyter Notebook**: For interactive development and demonstration.
*   **LangChain**: A framework for developing applications powered by language models.
*   **OpenAI**: Used for generating text embeddings and for the LLM.
*   **ChromaDB**: An open-source vector database for local development.
*   **Pinecone**: A managed vector database for scalable, production-ready applications.
*   **Pandas**: For data manipulation.

## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/sriharsha-nemalikonda/genai-rag-finance.git
    cd genai-rag-finance
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Set up your API keys:**
    Create a `.env` file in the root directory and add your OpenAI and Pinecone API keys:
    ```
    OPENAI_API_KEY=your_openai_api_key
    PINECONE_API_KEY=your_pinecone_api_key
    PINECONE_ENVIRONMENT=your_pinecone_environment
    ```
4.  **Run the Jupyter notebook:**
    ```bash
    jupyter notebook notebook.ipynb
    ```