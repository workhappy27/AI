#### What is a Retrieval Augmented Generation (RAG)?  
 - Retrieval, a system that retrieves the information  
 - Augmented, augment the information to be passed 
 - Generation, finally generate the information

#### RAG Triad 
Retrieval-Augmented Generation

```mermaid
flowchart LR
    Q[Query] --> R[Query]
    R --> C[Context]
    C --> Q[Response]
```

 - Context Relevance, is the retrieved Context relevant to the Query?
 - Groundness Relevance, is the Response supported by the Context?
 - Answer Relevance, is the Response relevant to the Query?
