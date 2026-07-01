#### Prompt Engineering Techniques:  
 - Zero Short  Prompting  
 - Few-shot Prompting
 - Chain-of-Through (CoT)
 - Self-Consistency
 - Knowledge Generation
 - Tree of Thoughts (ToT)  
   
#### Zero Short Prompting  
- Zero short prompting is without showing example of what a solution might look like.
- One can use this as the first try at a model
- Classify the sentiment in this sentence as negative or positive.

#### Few-Shot
 - Show model few examples of what a solution might look like.

#### Chain-of-Thought  
 - Enables complex reasoning capabilities through intermediate reasoning steps.
 - Examples: Reasoning aptitue questions.
 - Example-1:  
   Ask a Question, example of an answer showing intermediate reasoning steps that lead to a solution, and then prime the model with similar type, category, group to get response.
 - Example-2:
   Zero shot chain of though using same model as used in Example-1.


#### Self-Consistency  
 - Providing many solutions to get final answer.
 - Elicit reasoning and response.  
 - Many ways to think through a problem, getting the solutions which has majority votes.
 - Examples:  
 - Exmaple-1:
   a. Limiting the number of responses to 10.
   b. Prompting the model to using a chain of thought.
   c. Replace greedy decode in CoT prompting by samplig from the language's model's decoder to generate diverse set of reasoning paths.
   d. Marginalize the reasoning paths and aggregate by chosing most consistent answer in the ifnal answer set.
   Consistency in the output is going to be the defining factor for chosing the best response.  That's Self-Consistency.

#### Knowledge Generation  
 - Knowledge Generation: Generating facts related to the question.  
 - Knowledge Integration: Using genereated facts to answer the question.

 #### Tree of Thoughts  
  - ToT allows LMs to perform delierate decision making by considering multiple different reasoning paths and self-evaluating choices to decide the next course of action.  
   
