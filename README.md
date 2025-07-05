# AI PDF Chatbot & Agent Powered by LangChain and LangGraph

![GitHub Release](https://img.shields.io/badge/Release-Check%20Latest-brightgreen) [![GitHub](https://img.shields.io/badge/GitHub-Repo-blue)](https://github.com/guahusni/ai-pdf-chatbot-langchain/releases)

## Table of Contents

1. [Features](#features)
2. [Architecture Overview](#architecture-overview)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Environment Variables](#environment-variables)
   - [Frontend Variables](#frontend-variables)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)

## Features

- **PDF Ingestion**: Seamlessly ingest PDF documents for analysis.
- **Vector Database**: Store embeddings in Supabase for efficient querying.
- **User Queries**: Respond to user questions using OpenAI or other LLMs.
- **Customizable**: Tailor the chatbot to meet specific needs.
- **Integration**: Leverage LangChain and LangGraph for orchestration.

## Architecture Overview

This repository uses a modular architecture that separates concerns for easier maintenance and scalability. The main components include:

- **Frontend**: A user-friendly interface that allows users to interact with the chatbot.
- **Backend**: Handles PDF ingestion, embedding storage, and query responses.
- **Vector Database**: Manages the embeddings for fast retrieval.
- **LLM Provider**: Utilizes OpenAI or another LLM for generating responses.

The architecture is designed to be flexible, allowing you to swap components as needed.

## Prerequisites

Before you start, ensure you have the following:

- Node.js (version 14 or higher)
- Python (version 3.7 or higher)
- A Supabase account
- An OpenAI API key (or alternative LLM provider)

## Installation

To set up the project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/guahusni/ai-pdf-chatbot-langchain.git
   cd ai-pdf-chatbot-langchain
   ```

2. **Install Dependencies**:
   For the frontend:
   ```bash
   cd frontend
   npm install
   ```

   For the backend:
   ```bash
   cd backend
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**:
   Create a `.env` file in the root directory and add the necessary variables. See the [Environment Variables](#environment-variables) section for details.

4. **Run the Application**:
   Start the backend server:
   ```bash
   cd backend
   python app.py
   ```

   Start the frontend server:
   ```bash
   cd frontend
   npm start
   ```

## Environment Variables

To configure the application, set the following environment variables in your `.env` file:

### Frontend Variables

- `REACT_APP_API_URL`: URL for the backend API.
- `REACT_APP_OPENAI_API_KEY`: Your OpenAI API key.

### Backend Variables

- `SUPABASE_URL`: Your Supabase project URL.
- `SUPABASE_KEY`: Your Supabase API key.
- `OPENAI_API_KEY`: Your OpenAI API key.

## Usage

Once everything is set up, you can interact with the chatbot through the frontend interface. Upload a PDF document, and the bot will analyze it. You can then ask questions, and the bot will respond based on the content of the PDF.

### Example Interaction

1. Upload a PDF document.
2. Ask questions like:
   - "What is the main topic of the document?"
   - "Can you summarize the second section?"
3. The bot will provide answers based on the document's content.

## Contributing

We welcome contributions! To get started:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add some feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/YourFeature
   ```
5. Create a pull request.

Please ensure your code adheres to the existing style and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [LangChain](https://langchain.com) for providing the orchestration framework.
- [LangGraph](https://langgraph.com) for facilitating the integration of language models.
- OpenAI for their powerful language model API.
- Supabase for the vector database solution.

For more details, check the [Releases](https://github.com/guahusni/ai-pdf-chatbot-langchain/releases) section for updates and downloadable files.