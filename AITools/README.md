# AI Tools, Examples

[![SWAN](https://swan.web.cern.ch/sites/swan.web.cern.ch/files/pictures/open_in_swan.svg)](https://swan-k8s.cern.ch/user-redirect/download?projurl=https://github.com/cerndb/NotebooksExamples.git)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cerndb/NotebooksExamples)

This folder contains Jupyter notebook examples of AI tools, including LLMs, Transformers, vector databases.
The notebooks are intended to be run using GPU resources.  
To use GPU resources in [SWAN](https://swan.web.cern.ch/), you need to
 - Access SWAN from you browser: https://swan.cern.ch 
 - Select a software stack with `GPU`
   - To get the latest version of the tools used here select the 'bleeding edge' software stack

Contact: Luca.Canali@cern.ch

## Transformers library for text, image, and speech
This is to illustrate the use of the Transformers library from Hugging Face for LLM, Natural Language Processing (NLP), image, and speech tasks.

* [Transformers for text classification](Transformers_text_example.ipynb)
* [Transformers for image classifier](Transformers_image_example.ipynb)
* [Stable diffusion with transformers](Transformers_stable_diffusion_example.ipynb)
* [Transformers for speech recognition](Transformers_speech_recognition.ipynb)

## Large Language Models
These notebooks provide examples of how to use LLMs in notebook environments for tests and prototyping
* [Transformers Large Language Models](Transformers_Large_Language_Models.ipynb)
* [LangChain LLMs](LangChain_LLMs.ipynb)

## Semantic search with Vector Databases and LLM
Semantic search allows to query a set of documents. This example notebook shows how to create
vector embeddings, store them in a vector database, and perform semantic queries enhanced with LLM.
* [Semantic search with Vector Databases and LLM](LangChain_OpenSearch_semantic_search_with_Vector_DB.ipynb)
