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
    A[Documents]

    subgraph Chunks
        B1[Chunk 1]
        B2[Chunk 2]
        B3[Chunk 3]
    end

    C[Embedding LLM]

    subgraph Embeddings
        D1[Embedding 1]
        D2[Embedding 2]
        D3[Embedding 3]
    end

    A --> B1
    A --> B2
    A --> B3

    B1 --> C
    B2 --> C
    B3 --> C

    C --> D1
    C --> D2
    C --> D3
```
