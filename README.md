# LangChain + Hugging Face Colab Starter

A lightweight, ready-to-run Google Colab notebook for running open-weights LLMs (like Llama 3.1 8B Instruct) using LangChain and Hugging Face Inference Endpoints.

No GPU or local setup required—just drop in your API key and start prompting.

---

## Features
- Serverless LLM Calls: Uses Hugging Face Serverless Inference Endpoints to query models without local hardware requirements.
- Secure Credentials: Leverages Google Colab's built-in userdata secret management to keep your API tokens private.
- Minimal Code: Clean, straightforward Python implementation using langchain-huggingface.

---

## Tech Stack
- Language: Python 3
- Frameworks: langchain, langchain-huggingface, huggingface_hub
- Model: meta-llama/Llama-3.1-8B-Instruct
- Environment: Google Colab

---

## Quick Start

### 1. Grab Your Hugging Face API Token
If you do not have one yet, generate a free User Access Token under your Hugging Face Settings.

### 2. Save Your API Key in Colab
1. Open your notebook in Google Colab.
2. Click the Secrets icon on the left sidebar.
3. Add a new secret:
   - Name: HUGGINGFACEHUB_API_TOKEN
   - Value: Your Hugging Face Token
4. Toggle Notebook access to ON.

### 3. Install and Run

Install the necessary dependencies:

```bash
pip install -q langchain langchain-huggingface huggingface_hub
