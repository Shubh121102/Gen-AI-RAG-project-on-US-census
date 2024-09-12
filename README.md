# Gen-AI-RAG-project-on-US-census
**Retrieval Augmented Generation project on US census data using Langchain, HuggingFace, Mistral LLM model and Chroma DB.**
First we make pip installs, then we import libraries including **Langchain**, **Huggingface**, **Mistral**, Sentence Transformers, Recursive Character Text Splitter and **Chroma DB**.
Then we load the data stored in pdf files. Then we use text splitter to split the text into small **chunks**. We store these chunks in the form of **embedding** vectors in the Chroma DB. We store it in a **retriever** and use **similarity** search and return **3** chunks for the relevant query to be performed.
Following this we import our **LLM** model **Mistralai** for which we configure our **API Token** stored in user data and create a **prompt template** where we use our prompt.
Finally we use our **RetrievalQA chain** to combine our LLM model,retriever model, prompt and use the chain type **stuff**.
We store our user query in a variable and fetch it using the invoke function. We store this **result** in a variable and print it to show the output. 
