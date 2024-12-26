# Chat with PDF using Gemini

Welcome to the Chat with PDF project! This project allows you to upload PDF files, extract their text, store the text in a vector database (using FAISS), and ask questions using a conversational model (Gemini).

## Overview

This project is built using Streamlit to provide an easy-to-use interface for users to interact with multiple PDF files. It leverages Retrieval-Augmented Generation (RAG) by using a retrieval system to find relevant documents and a generative model (Chat with Gemini) to answer questions based on the retrieved documents.

## Features

- **PDF Upload**: Upload PDF files to extract text.
- **Text Chunking**: Split the text from PDFs into smaller chunks for efficient retrieval.
- **Vector Database (FAISS)**: Store these text chunks in a vector database for fast retrieval.
- **Conversational Model (Gemini)**: Ask questions to the model based on the retrieved documents.
- **User Input**: Input questions in a text field, and get responses generated using the retrieved information.

## Prerequisites

Before you get started, make sure you have the following prerequisites:

- Python 3.7+
- Required Python packages (install via `pip`):
  ```bash
  pip install streamlit PyPDF2 langchain langchain-google-genai google-generativeai dotenv
  ```
- API Keys: Make sure to obtain API keys for services like Google Generative AI. Set your API keys in the environment variables.
```bash
GOOGLE_API_KEY='YOUR_API_KEY_HERE
```
- Make sure to create a .env file with your API key in the root directory.
## Setup
## Clone this repository:

```bash
git clone https://github.com/Saketh-Vadlamudi/ChatWithPDF.git
cd ChatWithPDF
```
## Install the required Python packages:

```bash
pip install -r requirements.txt
```
## Run the Streamlit app:

```bash
streamlit run app.py
```
Ensure your API keys and .env file are set up correctly. If required, adjust the app.py to load your specific configuration (like model settings or database paths).

## Usage
```bash
Upload PDF Files: Use the file uploader to upload your PDF documents.
Ask Questions: Input your questions in the text input field.
View Responses: Responses are generated based on the retrieved context and are displayed below the input.
```
