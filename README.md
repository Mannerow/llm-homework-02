# llm-homework-02

## 📄 Overview

This project demonstrates the integration of the `OpenAI API` with a locally running `Docker` container to generate text completions. The provided Jupyter Notebook, ollama.ipynb, guides users through setting up the environment, configuring the API connection, and running text generation queries using a custom Docker image. The notebook includes all necessary steps to pull the Docker image, configure the OpenAI client, and perform text generation tasks efficiently.

## 🔐 Authentication

To authenticate with the OpenAI API, create a `.env` file in the project directory and add your API key in the following format:

```bash
OPENAI_API_KEY=your-api-key-here
```