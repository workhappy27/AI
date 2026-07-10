#### Drawbacks of Naive RAG

- Limited contextual understnading
  a. focus on keyword matching or basic semantic search (retrieving irrelevant or partially relevant document)
  
 - Inconsistent relevance and quality of retrieved documents.
   a. Varying in quality and (outdated or less credible) relevance documents (Poor-quality inputs for the gen model)
   
 - Poor integration between retrieval and generation
   a. Retriver and generator to working NOT in sync (unoptimized information)
   
 - Inefficient handling of Large-Scale data
   a. Scaling issues, take too long to find relevant docs,  or miss critical info due to bad indexing 

 - Lack of robustness and adaptability
   a. Not adaptable to changing contexts or user needs without significant manual intervention

   #### Summary
   1. Retrieval Challenges
   2. Generative Challenges
