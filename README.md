# Chatbot from a website
### A Langchain chatbot with streamlit GUI
This project mainly focus on interacting with chatbot who learns everything from a given website. It leverages the capability for llms and vector databases to rag train the llm models as per own requirements. This project is a comprehensive guide to building a chatbot capable of interacting with websites, extracting information, and communicating in a user-friendly manner. It leverages the power of LangChain 0.1.0 and integrates it with a Streamlit GUI for an enhanced user experience.

## Features
- *Website Scraping* : The program scrapes the whole wesite text and also its metadata.
- *Large Language Model Integration* : Compatibility with models like GPT-4, Mistral, Llama2, and ollama. In this code I am using GPT-4, but you can change it to any other model.
  NOTE : Google gemini-pro model is not compatible with multi chat.
- *Streamlit GUI* : A clean and intuitive user interface built with Streamlit, making it accessible for users with varying levels of technical expertise.
- *Python-friendly* : Entire code is written in Python including the frontend with the help of streamlit

## Brief About RAG
A RAG bot is short for Retrieval-Augmented Generation. This means that we are going to "augment" the knowledge of our LLM with new information that we are going to pass in our prompt. We first vectorize all the text that we want to use as "augmented knowledge" and then look through the vectorized text to find the most similar text to our prompt. We then pass this text to our LLM as a prefix.
![HTML-rag-diagram](https://github.com/Herin98/Website-ChatBot-LLM/assets/142152236/ff72067b-5f87-4724-b814-ae82b4161b0f)

## Installation
Ensure Python3.10 or above is install on your system. 
- Streamlit only supports upto 1.12.0 in py3.9. And streamlit chat_input is introduced after 1.24.0
- Langchain and langchain agents only compatible after py3.8
- Create a virtual env
- Run requirements.txt with compatible version
- Create your own .env file and add your api key

## Usage
After installation, to run streamlit app: ```streamlit run app.py```

### Additional
Feel free to star, fork, comment on this project. 
Ideas to add to this project:
- Same RAG concept can be used and instead of webscrapping, pdf/word reader can be used and the model can be trained on that data.
