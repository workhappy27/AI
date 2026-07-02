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
