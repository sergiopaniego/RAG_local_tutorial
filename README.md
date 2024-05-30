# Tutorial for RAG usage with an LLM locally or in Google Colab
Simple RAG tutorial that can be run locally or using Google Colab (only Pro version)

This notebook can be executed in local or in Google Colab. 
Either way, you have to install Ollama to run it.

# Technologies used

For this tutorial, we use LangChain for generating the RAG application code, Ollama for serving the LLM model and a Jupyter or Google Colab notebook

<p align="center">
  <img src="https://cdn.analyticsvidhya.com/wp-content/uploads/2023/07/langchain3.png" alt="Langchain Logo" width="20%">
  <img src="https://bookface-images.s3.amazonaws.com/logos/ee60f430e8cb6ae769306860a9c03b2672e0eaf2.png" alt="Ollama Logo" width="20%">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" alt="Jupyter Logo" width="20%">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Google_Colaboratory_SVG_Logo.svg/1280px-Google_Colaboratory_SVG_Logo.svg.png" alt="Google Colab Logo" width="20%">
</p>


# Intructions to run the example locally

* Download and install Ollama: 

Go to this URL and install it: https://ollama.com/download

* Pull the LLM model. In this case, gemma:7b

```
ollama pull gemma:7b
```


# Intructions to run the example using Google Colab (Pro account needed)

<a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/example_rag.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

* Install Ollama from the command line:

(Press the button on the bottom-left part of the notebook to open a Terminal)

```
curl -fsSL https://ollama.com/install.sh | sh
```

* Pull the LLM model. In this case, gemma:7b

```
ollama serve & ollama pull gemma:7b
```

* Serve the model locally so the code can access it.

```
ollama serve & ollama run gemma:7b
```


If an error is raised related to docarray, refer to this solution: https://stackoverflow.com/questions/76880224/error-using-using-docarrayinmemorysearch-in-langchain-could-not-import-docarray

