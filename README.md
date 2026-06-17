# Turn Any LLM Into Expert - Simple Python RAG Project For Beginners
A step by step pipeline of Retrieval-Augmented Generation with Ollama, Langchain, FAISS.

What if we could take a language model, and turn it into an expert on something it has never seen before? Not by teaching it, but by giving it fast access to documents.
Like - a serious investigation into whether **Lord Elrond** is secretly **Agent Smith**. And that’s exactly what we’ll do today!

We'll take a tiny language model, and we will give it access to witness reports, testimonies, and forensic evidence - coding a proper RAG pipeline from start to finish. We will turn our model into a brilliant investigator fully familiar with the case. 

We will learn about chunking, embeddings, vector databases and retrieval, using 10 fan fiction documents I created for this project (checkout the `data` directory 😉). We’ll plug in Ollama, LangChain, FAISS and tiny Qwen - giving you a solid foundation for building your own expert systems. 

By the end of the video, you will fully understand the RAG process and how to make hilarious projects with your new set of skills 💪.

## Video Tutorial 🎥
<a href="https://youtu.be/oZYlrooPgvs" target="_blank"><img width="600" alt="RAG Python Project thumbnail" src="https://github.com/user-attachments/assets/2be4c4ba-7013-446b-81e2-a571caf502a7" /></a>

## What You'll Learn

- 📄 Loading PDF documents with LangChain
- ✂️ Splitting documents into chunks
- 🧠 Creating embeddings with Ollama
- 🗄️ Building a FAISS vector database
- 🔍 Retrieving relevant information
- 🤖 Turning Qwen into an expert with RAG
- 💬 Adding chat history
- 🎭 Giving your model an identity
- ⚡ Running RAG on GPU

## Environment Setup (in WSL):

1. Install Ollama:
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

**NOTE:** If the official installation command changed, you can find the new one here: [Official Ollama Installation For Linux](https://ollama.com/download/linux)

2. Dowload Models (Chat Model & Embeddings Model):
```bash
ollama pull qwen2.5:1.5b
ollama pull bge-m3
```

3. Set up Working Environemnt:
```bash
conda create -n rag_env python=3.12
conda activate rag_env
```
## Install Requirements
Choose which device you would like to run the workflow on - an NVIDIA CUDA based GPU or your CPU, and install requirements accordingly:

### Requirements For CPU Workflow
```bash
pip install \
    langchain \
    langchain-community \
    langchain-ollama \
    langchain-text-splitters \
    faiss-cpu \
    pypdf \
    jupyter
```

### Requirements For GPU Workflow

```bash
conda install -c pytorch -c nvidia -c conda-forge faiss-gpu=1.14.3
```

**NOTE:** If the official installation command changed, you can find the new one here: [Installing Faiss via Conda](https://github.com/facebookresearch/faiss/blob/main/INSTALL.md)

```bash
pip install \
    langchain \
    langchain-community \
    langchain-ollama \
    langchain-text-splitters \
    pypdf \
    jupyter
```

## Launch Jupyter And Run Your Workflow:

```bash
jupyter lab
```
