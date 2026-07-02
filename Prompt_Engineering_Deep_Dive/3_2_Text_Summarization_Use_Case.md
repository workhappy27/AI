#### Test Summarization Use Case
1. Define your task clearly
2. Define an evaluation metric
3. Generate prompt candidates
4. Experiment
5. Settle on a requires performace threshold to step experimentation.

#### Define our task  
 - Summarize research papers.
 - Summarize the main findings and methodology of the following paper.

#### Evaluation metric   
 - ROUGE: Recall-Oriented Understudy for Gisting Evaluation
 - BLEU: Bilingual Evaluation Understudy
 - METEOR: Metric or Evaluation of Translation with Explicit Ordering
 - BERTScore
 - LEPOR: Lenght Penalty, Overlap and Recall

Leverages GPT-4 as a judge for the quality of the summarization outputs obtained by using the following creteria.  
- Revelance
- Coherence
- Consistency
- Fluency

#### Simplied versionof experimentation pipeline
## Evaluation Loop85 86```mermaid87flowchart TD88 89    A[Prompt]90    --> B[Generate Summaries]91 92    B --> C[GPT-4 Evaluation]93 94    C --> D{Score >= Threshold?}95 96    D -- Yes --> E[Keep Candidate]97 98    D -- No --> F[Extract Feedback]99    F --> G[Prompt Refinement]100    G --> A101```
