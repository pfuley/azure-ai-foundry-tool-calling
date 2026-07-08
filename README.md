# Azure AI Foundry Tool Calling

A Python project demonstrating tool calling with Azure AI Foundry and the Azure OpenAI Responses API.

## Overview

This project demonstrates how to build a generative AI application that uses tools to extend model capabilities.

The application will use:

- Azure AI Foundry
- Azure OpenAI Responses API
- Microsoft Entra ID authentication
- Web Search
- File Search
- Vector Stores
- Retrieval-Augmented Generation style grounding

## Features

Current progress:

- ✅ Project structure
- ✅ Environment configuration
- ✅ Azure OpenAI client setup
- ✅ Vector store creation
- ✅ Brochure PDF upload
- ✅ Multi-turn conversation support
- ✅ Tool calling with the Responses API
- ✅ File Search tool
- ✅ Web Search tool

## Tech Stack

- Python
- Azure AI Foundry
- Azure OpenAI
- OpenAI Python SDK
- Azure Identity
- Python Dotenv

## Project Structure

```text
azure-ai-foundry-tool-calling/
├── brochures/
│   └── *.pdf
├── screenshots/
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
├── LICENSE
└── README.md
```

## Prerequisites

Before running this project, install:

- Python 3.13
- Git
- Azure CLI
- Visual Studio Code
- Active Azure subscription
- Azure AI Foundry project
- Deployed Azure OpenAI model

## Setup

Clone the repository:

```bash
git clone https://github.com/pfuley/azure-ai-foundry-tool-calling.git
cd azure-ai-foundry-tool-calling
```

Create and activate a virtual environment:

```bash
python -m venv .venv
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file using `.env.example`:

```env
AZURE_OPENAI_ENDPOINT=your_azure_openai_endpoint
MODEL_DEPLOYMENT=your_model_deployment_name
```

Sign in to Azure:

```bash
az login
```

Add travel brochure PDFs to the `brochures/` folder.

Run the app:

```bash
python app.py
```

Expected output:

```text
Azure OpenAI client initialized successfully.
Model deployment: your_model_deployment_name
Creating vector store and uploading files...
Vector store created with 3 files.
```

## Environment Variables

| Variable | Description |
|---|---|
| `AZURE_OPENAI_ENDPOINT` | Azure OpenAI endpoint from the Azure AI Foundry project home page |
| `MODEL_DEPLOYMENT` | Name of the deployed model in Azure AI Foundry |

## How File Search Will Work

The application uploads PDF brochures into a vector store.

Later, the `file_search` tool will use this vector store to answer questions about Margie's Travel services, hotels, and brochures.

## Learning Objectives

- Implement tool calling with the Azure OpenAI Responses API
- Build a multi-turn conversational AI application
- Ground AI responses using web search and vector-based file retrieval
- Understand how AI agents orchestrate external tools to answer user queries

## Acknowledgements

This project was developed as a personal learning exercise inspired by the Microsoft Learn lab **Create a generative AI app that uses tools**.

Reference:

```text
https://github.com/microsoftlearning/mslearn-ai-studio
```

## License

This project is licensed under the MIT License.