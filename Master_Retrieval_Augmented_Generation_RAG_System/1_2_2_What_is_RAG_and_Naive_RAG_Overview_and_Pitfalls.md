#### Componenets of RAG
 - Retriever
    - Identifies and retrieves relevant documents.
 - Generator
    - Takes retrieved docs and the input query to generate coherent and contextually relevant response

#### What is a RAG?
 -  - Definition a framework that combines the strengths of retrieval-based systems and generation-based model to produce more accurate and contextual relevant response.
  
    #### LLM
    - LLM knows what it was trained on. After injecting user input data, now LLM know some specific contextual data.

#### RAG Overview 

```mermaid
flowchart TD
     A[Documents] --> B[Chunk-1] [chunk-2] [Chunk-3] -->C[Embedding LLM] -->D[Emb-1] [Emb-2] [Emb-3]
```
