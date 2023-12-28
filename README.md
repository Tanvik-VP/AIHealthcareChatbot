# AIHealthcareChatbot

# Medical Bot

The Medical Bot is a powerful question-answering system built on top of state-of-the-art natural language processing models. It can retrieve answers from a database of documents by creating embeddings and utilizing the Llama model for enhanced response generation. This bot is particularly useful for addressing medical-related queries using the provided data.

## Features

- **Document Ingestion**: Easily loads and processes PDF documents from a directory.
- **Advanced Text Splitting**: Splits documents into chunks for better embedding.
- **Embedding Generation**: Uses the HuggingFace's Sentence Transformers to generate embeddings.
- **Efficient Vector Database**: Utilizes FAISS for efficient similarity search on embeddings.
- **Retrieval-based QA**: Uses RetrievalQA to fetch answers based on similarity and context.
- **Chainlit Integration**: Provides a chat-based interface for interactive usage.

## Setup

### Prerequisites

1. Python 3.7 or later.
2. Make sure to download the `llama-2-7b-chat.ggmlv3.q8_0.bin` model from HuggingFace. [ https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML] 
3. Install chain lit using `pip install chainlit`
4. Install faiss using `pip install faiss-cpu`
5. Install langchain using `pip install langchain`

## Download the data from the repo

## Usage

1. First, you'll want to create the vector database from your data:
   ```bash
   python ingest.py
2. Once the database is ready, you can run the chatbot interface:
   ```bash
   chainlit run model.py
3. Interact with the bot and get answers to your medical queries.

## Getting Started with AIHealthcareChatbot

To get started with the AIHealthcareChatbot, follow these steps:

### 1. Environment Setup

- Set up your environment and install all necessary packages. Refer to the **Installation** section for detailed instructions.

### 2. Configuration

- Modify the `DB_FAISS_PATH` variable and any other necessary configurations within the code according to your requirements.

### 3. Model and Data Preparation

- Ensure you have the required language model and data set up as specified in the documentation.

### 4. Starting the Bot

- Run the provided Python script to initiate the bot, or integrate it within your desired application.

## Usage Instructions

To interact with the AIHealthcareChatbot and seek answers to medical-related queries, follow the guide below:

1. **Initiate the Bot**: Activate the bot either by running the provided Python script or via your application.

2. **Send a Query**: Pose a medical-related question to the bot.

3. **Receive Response**: The bot will generate an answer based on its database's information.

4. **Check Sources (if available)**: For certain responses, the bot will supply relevant sources alongside the answer.

5. **Customization**: You can tailor the bot to yield specific results based on the query and the context given.

## Contribution

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page].

## License

This project is under the MIT license.
