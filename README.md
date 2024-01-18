# Local PDF Chat Application with Mistral 7B LLM, Langchain, Ollama, and Streamlit

A PDF chatbot is a powerful tool capable of answering questions about a PDF file. This application utilizes Mistral 7B LLM, Langchain, Ollama, and Streamlit to create an interactive PDF chatbot. The system employs the Retrieval-Augmented Generation (RAG) concept, enhancing its generation capabilities by retrieving relevant information from an external knowledge base.

## Project Overview

### Dependencies
- **Mistral 7B LLM:** A large language model for understanding user queries.
- **Langchain:** A library for building conversational AI applications.
- **Ollama:** Allows running Mistral locally, simplifying model setup and configuration.
- **Streamlit:** A framework for creating interactive web applications with Python.

### How It Works
1. Upload a PDF file through the web interface.
2. The application analyzes the document using Langchain and Ollama.
3. The chatbot, powered by Mistral 7B, answers user queries about the PDF content.

## Running Mistral 7B Locally using Ollama 🦙

Ollama facilitates the local usage of large language models such as Mistral 7B. Follow the steps below for setup:

### For Mac and Linux Users:
1. Install Ollama by following the instructions in the [Ollama GitHub Repository](https://github.com/ollama/ollama) for Mac and Linux.

### For Windows Users:
1. Install WSL 2 by referring to the official Microsoft documentation: [Install WSL 2](https://docs.microsoft.com/en-us/windows/wsl/install).
2. Install Docker for Windows by following the official Docker documentation: [Install Docker for Windows](https://docs.docker.com/desktop/install/windows-desktop/).
3. Access Mistral using the Docker image provided [here](https://github.com/ollama/ollama#docker).

Now, run Mistral in the command line (CMD) using the following command:

```bash
docker exec -it ollama ollama run mistral
```

## Usage
#### NOTE: First install Ollama in docker and run mistral as stated above

1. Clone this repository:
   
 ```
 git clone https://github.com/SonicWarrior1/pdfchat.git
 ```
2. Install all the depenedencies :
   
```
pip install -r requirements.txt
```
3. Open terminal and run the following command:
```
streamlit run app.py
```
## Application Preview :
![image](https://github.com/SonicWarrior1/pdfchat/assets/73881129/32f9685b-f70e-48da-8e6f-9fdce1fdd0cc)
