
# Bhagavad Gita Chatbot

Overview
This repository houses the codebase for a cutting-edge Bhagavad Gita chatbot. The chatbot is designed to provide relevant responses to commonly asked questions about the Bhagavad Gita. The responses are generated using the LangChain generative AI framework, specifically leveraging the Llama2 model. For efficient storage and retrieval of vector embeddings, Pinecone is utilized. The frontend is developed using Flask, providing a seamless and user-friendly interface.

Features
Custom Data Responses: The chatbot is trained on custom data to provide meaningful and contextually appropriate responses to user queries.
LangChain Generative AI: Utilizing the state-of-the-art LangChain framework, with the Llama2 model, ensures the generation of high-quality responses.
Efficient Vector Storage: Pinecone is employed for storing vector embeddings, enabling fast and accurate retrieval of information.
Flask Frontend: The frontend is developed using Flask, offering a user-friendly interface to interact with the Bhagavad Gita chatbot.


# End-to-end-Bhagvat GeetaChatbot-using-Llama2

# Setup Instructions

Clone the repository

```bash
Project repo: https://github.com/
```

### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n geetachatbot python=3.8 -y
```

```bash
conda activate geetachatbot
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

```bash
# run the following command
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- Pinecone


