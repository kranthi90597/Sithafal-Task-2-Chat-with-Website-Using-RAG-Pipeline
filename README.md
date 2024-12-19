# Chat-with-Website-Using-RAG-Pipeline

## **Overview**
This project implements a **Retrieval-Augmented Generation (RAG) Pipeline** to allow users to query website content efficiently. The system:
1. **Crawls and scrapes data** from websites.
2. Generates **vector embeddings** for the website content using a pre-trained model.
3. Stores embeddings in a **FAISS vector database**.
4. Handles user queries to **retrieve relevant data** and generate context-aware responses.


## **Technologies Used**
- **Python** 
- **BeautifulSoup4** and **requests** for web scraping.
- **SentenceTransformers** for embedding generation.
- **FAISS** (Facebook AI Similarity Search) for vector database.
- **Large Language Model (Optional)** for response generation.


## **Directory Structure**
```
Sithafal_Task_2
├── Task_2/
|   ├── scrape_and_embed.py      # Crawls websites, scrapes data, and generates embeddings
|   ├── query_retrieve.py        # Accepts user queries and retrieves relevant documents
|   ├── generate_response.py     # (Optional) Generates detailed responses using an LLM
|   ├── documents.txt            # Raw scraped website content
|   ├── website_embeddings.index # FAISS index storing embeddings
|   └── retrieved_docs.txt       # Contains top retrieved documents
└──requirements.txt              # Required installations are mentioned in this
```

## **How to Run the Project**
1. Clone the repository:
```
git clone https://github.com/kranthi90597/Sithafal-Task-2-Chat-with-Website-Using-RAG-Pipeline.git
cd Sithafal-Task-2-Chat-with-Website-Using-RAG-Pipeline
```
2. Install required libraries using ```pip```:
```
pip install -r requirements.txt
```
3. Run the following Scripts orderly:
```
python scrape_and_embed.py
python query_retrieve.py
python generate_response.py
```

## **Output Demonstration**
Enter the queries and get the answers

Example Queries
```
1. What is the university of Chicago known for?
2. Tell me about Stanford University?
```


## **Below are the Snapshots of the Output**

1. **After Executing ```python scrape_and_embed.py``` file**

    ![Scraping the data from websites](https://github.com/user-attachments/assets/3dca3ad6-09db-4870-8548-055a387c1eac)


2. **After running ```python query_retrive.py``` file**

    ![User Entering queries and getting answers](https://github.com/user-attachments/assets/49527f14-e915-412b-8795-d1166f7d1059)


3. **After executing ```python generate_response.py``` file**
   
    ![Generating response using LLMs](https://github.com/user-attachments/assets/e52f45ad-f9b1-41aa-8f4e-8e0a1bc12299)


## **Feel free to ask your valuable doubts**:

Email: kranthi90597@gmail.com

