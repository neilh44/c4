# ChatPDF README

## Overview

The `ChatPDF` project is a Python application built using the Streamlit framework and the Langchain library. It provides a simple interface for users to interact with a question-answering chatbot that leverages a PDF document for context retrieval.

## Files

### app.py

This file contains the Streamlit application code. The main functionalities include:

- **Display Messages:** Renders user and assistant messages in a chat-like interface.
- **Process Input:** Handles user input, invokes the assistant's response, and updates the chat display.
- **Read and Save File:** Manages file uploading, saves the PDF document temporarily, and triggers the assistant's ingestion process.

### rag.py

This file defines the `ChatPDF` class, which encapsulates the chatbot's functionality. Key components include:

- **Initialization:** Sets up the chatbot using Langchain components, such as `ChatOllama` for question-answering and `RecursiveCharacterTextSplitter` for text splitting.
- **Ingest:** Processes a PDF document, splits it into chunks, and creates a vector store for retrieval.
- **Ask:** Invokes the chatbot to respond to user queries based on the ingested context.
- **Clear:** Resets the chatbot's internal state.

## Dependencies

The project relies on the following Python libraries:

- Streamlit
- Langchain

Ensure these libraries are installed in your Python environment before running the application.

## How to Run

1. Install dependencies using `pip install streamlit langchain`.
2. Run the Streamlit app with `streamlit run app.py`.
3. Upload a PDF document to initiate the chatbot and start interacting.

## Note

- The application is designed for question-answering tasks based on the content of uploaded PDF documents.
- The Langchain library is used for text processing, document loading, and question-answering model integration.

Feel free to explore and customize the code to suit your needs!
