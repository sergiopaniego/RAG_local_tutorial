# Tutorials for RAG usage with an LLM locally or in Google Colab

Simple RAG tutorials that can be run locally with an LLM or using Google Colab (only Pro version).

These notebooks can be executed in local or in Google Colab. 
Either way, you have to install Ollama to run it.

<img src="./imgs/rag_diagram.png" alt="RAG diagram"/>

# Tutorials

* [Extracting details from a file (PDF) using RAG](./example_rag.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/example_rag.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

* [Extracting details from a YouTube video using RAG](./youtube_rag.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/youtube_rag.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

* [Extracting details from an audio using RAG](./whisper_rag.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/whisper_rag.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

* [Extracting details from a GitHub repo using RAG](./github_repo_rag.ipynb) <a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/github_repo_rag.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# Technologies used

For this tutorials, we use LangChain, LlamaIndex and HuggingFace for generating the RAG application code, Ollama for serving the LLM model and a Jupyter or Google Colab notebook.

<p align="center">
  <img src="https://cdn.analyticsvidhya.com/wp-content/uploads/2023/07/langchain3.png" alt="Langchain Logo" width="15%">
  <img src="https://images.contentstack.io/v3/assets/bltac01ee6daa3a1e14/blt45d9c451c9a70269/6542d10b8b3f8e001b7aeead/img_blog_image_inline.png?width=1120&disable=upscale&auto=webp" alt="LlamaIndex Logo" width="15%">
  <img src="https://huggingface.co/datasets/huggingface/brand-assets/resolve/main/hf-logo-with-title.png" alt="HuggingFace Logo" width="15%">
  <img src="https://bookface-images.s3.amazonaws.com/logos/ee60f430e8cb6ae769306860a9c03b2672e0eaf2.png" alt="Ollama Logo" width="15%">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" alt="Jupyter Logo" width="15%">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Google_Colaboratory_SVG_Logo.svg/1280px-Google_Colaboratory_SVG_Logo.svg.png" alt="Google Colab Logo" width="15%">
</p>


# Intructions to run the example locally

* Download and install Ollama: 

Go to this URL and install it: https://ollama.com/download

* Pull the LLM model. In this case, llama3:

```
ollama pull llama3
```

More details about llama3 in the [official release blog](https://llama.meta.com/llama3/) and in [Ollama documentation](https://ollama.com/library/llama3).

# Intructions to run the example using Google Colab (Pro account needed)

* Install Ollama from the command line:

(Press the button on the bottom-left part of the notebook to open a Terminal)

```
curl -fsSL https://ollama.com/install.sh | sh
```

* Pull the LLM model. In this case, llama3

```
ollama serve & ollama pull llama3
```

* Serve the model locally so the code can access it.

```
ollama serve & ollama run llama3
```


If an error is raised related to docarray, refer to this solution: https://stackoverflow.com/questions/76880224/error-using-using-docarrayinmemorysearch-in-langchain-could-not-import-docarray


