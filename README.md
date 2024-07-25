# Hybrid Search RAG Pipeline in LlamaIndex

This project demonstrates the implementation of a Hybrid Search Retrieval Augmented Generation (RAG) pipeline using open source models from `Hugging Face` and `FastEmbeddings` integrated with `llama-index`. The goal is to enhance the retrieval and generation capabilities for complex search queries, particularly in the domain of medical documents.

## Overview

### Concept

A Hybrid Search RAG pipeline combines the strengths of traditional keyword-based search and modern vector-based search. This approach leverages pre-trained language models to improve the accuracy and relevance of search results by understanding the semantic meaning of queries and documents.

### Components

1. **Hugging Face Models**: Utilized for their powerful language models and APIs which allow for advanced text generation and understanding.
2. **FastEmbeddings**: Employed for efficient and accurate text embedding, enabling the transformation of text data into numerical vectors that capture semantic information.
3. **LlamaIndex**: Acts as the core framework, integrating vector stores, document processing, and query handling to facilitate the creation of sophisticated search pipelines.

### Architecture

1. **Data Ingestion**: Load and preprocess medical documents for indexing.
2. **Embedding Generation**: Use FastEmbeddings to convert text data into high-dimensional vectors.
3. **Indexing**: Store the generated embeddings using Chroma, a vector store optimized for handling large-scale data.
4. **Query Processing**: Employ Hugging Face language models to interpret and generate responses to user queries.
5. **Hybrid Search**: Combine vector similarity search with traditional keyword-based search to provide comprehensive search results.

## Use Cases

### Medical Research

Researchers can leverage this pipeline to search through vast repositories of medical documents, retrieving relevant studies, articles, and reports that match their queries both semantically and contextually.

### Clinical Decision Support

Healthcare professionals can utilize the system to quickly find information on medical conditions, treatment protocols, and drug interactions, aiding in making informed clinical decisions.

### Knowledge Management

Organizations can deploy the pipeline to manage and retrieve internal documents, ensuring that employees have access to the most relevant and up-to-date information for their needs.

### Educational Purposes

Students and educators can use the hybrid search capabilities to find educational materials, research papers, and other academic resources that align closely with their study topics.

## Benefits

- **Improved Search Accuracy**: By combining vector and keyword search, the pipeline offers more precise and contextually relevant results.
- **Scalability**: The use of Chroma for vector storage allows the system to handle large datasets efficiently.
- **Flexibility**: The integration of multiple open-source tools provides a customizable and extensible framework for various applications.

## Getting Started

To start using this pipeline, you will need to set up the necessary environment, including installing the required packages and configuring access tokens for Hugging Face APIs. Once set up, you can ingest your document data, generate embeddings, and start performing hybrid searches.

## Future Work

- **Enhanced Model Integration**: Incorporate additional language models and embedding techniques to further improve search capabilities.
- **Domain Expansion**: Adapt the pipeline for other domains beyond medical, such as legal or technical documentation.
- **User Interface**: Develop user-friendly interfaces to make the system accessible to non-technical users.
