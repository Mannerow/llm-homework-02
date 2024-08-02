# llm-homework-02

## 📄 Overview

This project integrates the OpenAI API with a locally running Docker container to generate text completions using the `gemma:2b` model. The provided Jupyter Notebook, `ollama.ipynb`, guides users through environment setup, API configuration, and text generation. Users can pull the Docker image, configure the OpenAI client, and execute text generation tasks. To run the Docker container, use `docker run -it --rm -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama` and verify with `docker ps`. Enter the container with `docker exec -it ollama ollama pull gemma:2b` and test prompts. To persist model weights, map `/root/.ollama` to a local directory instead of a named volume.

## 🔐 Authentication

To authenticate with the OpenAI API, create a `.env` file in the project directory and add your API key in the following format:

```bash
OPENAI_API_KEY=your-api-key-here
```