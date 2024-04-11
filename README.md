# RAG_local_tutorial
Simple RAG tutorial that can be run locally or using Google Colab (only Pro version)

This notebook can be executed in local or in Google Colab. 
Either way, you have to install Ollama to run it.

# Intructions to run the example locally

* Download and install Ollama: 

Go to this URL and install it: https://ollama.com/download

* Pull the LLM model. In this case, gemma:7b

```
ollama pull gemma:7b
```


# Intructions to run the example using Google Colab (Pro account needed)

<a target="_blank" href="https://colab.research.google.com/github/sergiopaniego/RAG_local_tutorial/blob/main/example.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

* Install Ollama from command line:

(Press the button on the bottom-left part of the notebook to open a Terminal)

```
curl -fsSL https://ollama.com/install.sh | sh

ollama
```

* Pull the LLM model. In this case, gemma:7b

```
ollama pull gemma:7b
```

* Serve the model locally so the code can access it.

```
ollama serve & ollama run gemma:7b
```
