# Research Agent with Memory

An agent created to facilitate research on ArXiv platform.

## Functionalities

Search interface for querying arXiv papers
AI-powered processing of search results for improved readability
Persistent memory of user interests and past searches
Utilizes OpenAI's GPT-4o-mini model for intelligent processing
Implements memory storage and retrieval using Mem0 and Qdrant

## Installation

1. Download or clone repository
2. Install necessary files with pip install -r requirements.txt
3. The app expects Qdrant to be running on localhost:6333. Adjust the configuration in the code if your setup is different.

docker pull qdrant/qdrant

docker run -p 6333:6333 -p 6334:6334 \
    -v $(pwd)/qdrant_storage:/qdrant/storage:z \
    qdrant/qdrant
    
4. Run the application with streamlit run arxiv_research_agent.py