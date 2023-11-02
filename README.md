# Local PDF Chat Application with Mistral 7B LLM, Langchain, Ollama, and Streamlit

A PDF chatbot is a chatbot that can answer questions about a PDF file. It can do this by using a large language model (LLM) to understand the user's query and then searching the PDF file for the relevant information. The application uses the concept of Retrieval-Augmented Generation (RAG) to generate responses in the context of a particular document. RAG applications augment their generation capabilities by retrieving relevant information from an external knowledge base. This allows RAG applications to produce more informative and comprehensive responses to a wider range of prompts and questions.

## Running Mistral 7B Locally using Ollama 🦙

Ollama allows you to run open-source large language models, such as Llama 2, locally. It bundles model weights, configuration, and data into a single package, defined by a Modelfile, optimizing setup and configuration details, including GPU usage.

**For Mac and Linux Users:**
Ollama effortlessly integrates with Mac and Linux systems, offering a user-friendly installation process. Mac and Linux users can swiftly set up Ollama to access its rich features for local language model usage. Detailed instructions can be found here: [Ollama GitHub Repository for Mac and Linux](https://github.com/ollama/ollama).

**For Windows Users:**
For Windows users, the process involves a few additional steps, ensuring a smooth Ollama experience:

1. **Install WSL 2:** To enable WSL 2, kindly refer to the official Microsoft documentation for comprehensive installation instructions: [Install WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install).

2. **Install Docker:** Docker for Windows is a crucial component. Installation guidance is provided in the official Docker documentation: [Install Docker for Windows](https://docs.docker.com/desktop/install/windows-install).

3. **Utilize Docker Image:** Windows users can access Ollama by using the Docker image provided here: [Ollama Docker Image](https://hub.docker.com/r/ollama/ollama).

Now you can easily use Mistral in the command line (CMD) using the following command:

```
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
