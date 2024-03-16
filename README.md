# Movie Recommender RAG system

### Description

Leveraged Google's open-source Gemma model to design and implement a personalized movie recommendation engine, enhancing user experience through tailored content.

Integrated MongoDB for vector-based database management, significantly improving the system's recommendation accuracy and performance.

### Motivation
The rise of Generative AI comes with a great appreciation of personalization, that is, the ability to create unique experience for each users. We will see how open source and Gen AI transform the way we do recommendation system in near future.

Google's open source model Gemma is my top choice due to its small model parameters and good performance. A lighter requirement on compute resources. In the year of 2024, small language model (SLM) is the trend.

### Workflow
![image](https://github.com/weibb123/RAG_movie_recommender/assets/84426364/4de7e26c-56ea-49d0-8e55-eb2e6d1e76eb)
![image](https://github.com/weibb123/RAG_movie_recommender/assets/84426364/d014ac07-3339-4644-bfa6-c8274ac51799)

### Tech Stack
MongoDB: Connect to clusterA Python library for interacting with MongoDB that enables functionalities to connect to a cluster and query data stored in collections and documents.
MongoDB also support vector database store and has tutorial on how to define vector search pipeline. Also, converting from python dataframe to json-like collection in MongoDB is easy process.

Pandas: Data preparation in python dataframe

Hugging Face Accelerate: Abstracts the complexity of writing code that leverages hardware accelerators such as GPUs. Accelerate is leveraged in the implementation to utilise the Gemma model on GPU resources.

Hugging Face Transformers: Access to a vast collection of pre-trained models

Hugging Face Sentence Transformers: Provides access to sentence, text, and image embeddings.

utilized Google open source model Gemma, embedding to create RAG system with mongoDB

### What's Next
The choice of your LLM will change the setup of the code. Google Colab is able to fit Gemma-2B with Tesla V4. 
To run it locally, **llama-cpp-python** supports users to use LLM without beast machines.

Integrate in a bigger software by writing a web server using FASTAPI. Host the LLM on cloud. store newer data to database. 
