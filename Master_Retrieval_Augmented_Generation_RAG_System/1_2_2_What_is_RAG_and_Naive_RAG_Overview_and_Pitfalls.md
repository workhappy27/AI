#### Componenets of RAG
 - Retriever
    - Identifies and retrieves relevant documents.
 - Generator
    - Takes retrieved docs and the input query to generate coherent and contextually relevant response

#### What is a RAG?
 - Definition a framework that combines the strengths of retrieval-based systems and generation-based model to produce more accurate and contextual relevant response.
  
    #### LLM
    - LLM knows what it was trained on. After injecting user input data, now LLM know some specific contextual data.

#### RAG Overview 
The generated data is augmented by the data the system retrieved from the documents.  

```mermaid
flowchart TD
    A[Documents]

    subgraph Chunks
        B1[Chunk 1]
        B2[Chunk 2]
        B3[Chunk 3]
    end

    Q[Query]

    C[Embedding LLM]

    subgraph Embeddings
        D1[Embedding 1]
        D2[Embedding 2]
        D3[Embedding 3]
    end

    QE[Query Embedding]

    MS[Most Similar]

    G[Gen. LLM]

    R[Response]

    A --> B1
    A --> B2
    A --> B3

    B1 --> C
    B2 --> C
    B3 --> C

    Q --> C
    C --> QE

    C --> D1
    C --> D2
    C --> D3

    D1 --> MS
    D2 --> MS
    D3 --> MS

    QE --> MS

    MS --> G
    G --> R
```

#### Naive RAG
 - Most simple RAG dealing with LLM


```mermaid
flowchart TB

subgraph Process
direction LR

I[Indexing]
R[Retrieval]
G[Generation]
end

I --- ID["Cleaning<br/>extracting data<br/>from docs or DB"]

R --- RD["Turn question into<br/>Vector comparison<br/>Retrives closely<br/> Related chunk.."]

G --- GD["The query, choose docs<br/>combined into a prompt<br/>The model generates<br/n> an answer"]
```
