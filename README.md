# Azure AI Foundry Tool Calling

A Python project demonstrating how to build an AI application using **Azure AI Foundry** and the **Azure OpenAI Responses API** with tool calling capabilities.

## Features

- Azure AI Foundry integration
- Azure OpenAI Responses API
- Tool Calling
- Web Search
- File Search
- Vector Store integration
- Microsoft Entra ID authentication

## Tech Stack

- Python
- Azure AI Foundry
- Azure OpenAI
- OpenAI Python SDK
- Azure Identity

## Project Structure

```text
tools-app/
├── brochures/
├── app.py
├── requirements.txt
├── .env.example
├── README.md
└── .gitignore
```

## Project Status

🚧 This project is being developed incrementally with meaningful Git commits to demonstrate the complete development process.
🚧 Project initialization and configuration completed.

Current progress:
- ✅ Project structure
- ✅ Environment configuration
- ✅ Azure authentication
- ✅ OpenAI client
- ⏳ Tool calling
- ⏳ File Search
- ⏳ Web Search

## Setup

1. Clone the repository.
2. Create a Python virtual environment.
3. Install the project dependencies:

```bash
pip install -r requirements.txt
```

4. Create a `.env` file using `.env.example`.
5. Add your Azure AI Foundry endpoint and model deployment name.

## Learning Objectives

- Build AI applications with Azure AI Foundry
- Authenticate using Microsoft Entra ID
- Use the Azure OpenAI Responses API
- Implement tool calling
- Ground responses with web search and file search
- Follow Git best practices with incremental commits

## License

This project is licensed under the MIT License.

## Acknowledgements

This project was developed as a personal learning exercise inspired by the Microsoft Learn lab **"Create a generative AI app that uses tools"**. The implementation in this repository was built independently while following the concepts and guidance provided by Microsoft Learn.

Reference:
https://github.com/microsoftlearning/mslearn-ai-studio