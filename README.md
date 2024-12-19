# Chat-with-Website-Using-RAG-Pipeline

## **Overview**
This project implements a **Retrieval-Augmented Generation (RAG) Pipeline** to allow users to query website content efficiently. The system:
1. **Crawls and scrapes data** from websites.
2. Generates **vector embeddings** for the website content using a pre-trained model.
3. Stores embeddings in a **FAISS vector database**.
4. Handles user queries to **retrieve relevant data** and generate context-aware responses.

---

## **Technologies Used**
- **Python** 
- **BeautifulSoup4** and **requests** for web scraping.
- **SentenceTransformers** for embedding generation.
- **FAISS** (Facebook AI Similarity Search) for vector database.
- **Large Language Model (Optional)** for response generation.

---

## **Directory Structure**
```plaintext
Task_2/
│
├── scrape_and_embed.py      # Crawls websites, scrapes data, and generates embeddings
├── query_retrieve.py        # Accepts user queries and retrieves relevant documents
├── generate_response.py     # (Optional) Generates detailed responses using an LLM
├── documents.txt            # Raw scraped website content
├── website_embeddings.index # FAISS index storing embeddings
└── retrieved_docs.txt       # Contains top retrieved documents
```

## **How to Run the Project**
Step-1
```
pip install -r requirements.txt
```
Step-2
Run the Scripts
```
python scrape_and_embed.py
python query_retrieve.py
python generate_response.py
```
## **Output Demonstration**
Enter the queries and get the answers

## **Below are the Snapshots of the Output**

1. After Executing ```python scrape_and_embed.py``` file
![scrape_and_embed](image-1.png)

2. After running ```python query_retrive.py``` file
![query_retrieval](image.png)

3. After executing ```python generate_response.py``` file
![generate_response](image-2.png)
