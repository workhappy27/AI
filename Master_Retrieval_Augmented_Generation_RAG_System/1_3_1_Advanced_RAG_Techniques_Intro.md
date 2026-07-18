#### Advanced RAG Techniques and their Solutions:  
 - Advanced RAG - Introduces specific improvements to overcome the limitations of Naive RAG. Focus on enhancing retrieval quality.

 ##### Advanced RAG employs the following strategies
1. Pre-retrieval  
   a. Improvement of the indesing strucure and user's query  
   b. Improves data details, organizing indexesbetter, adding extra information, aligning things correctly  

2. Post-retrieval  
   a. Combine pre-retrieval data with the original query
       Re-ranking to highlight the most important.  

##### Query Expansion (with generated answer)
 Generate potential answers to the query [using an LLM] and to get relevant context.  

**Use cases:**
- Information Retrieval
- Question Answering Systems
- E-Commerce Search
- Academic Search



```mermaid
flowchart LR

    A[User Query] --> B[LLM]
    B --> C[Answer]

    A --> D[Vector DB]
    C --> D

    D --> E[Query Results]
    E --> F[LLM]

    F --> G[Final Answer]
```
