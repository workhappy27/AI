#### Code Generation Use Case

1. Introduction:
   - Problem to be solved through LLMs like Chat-GPT4 to generate functional python code for basic calculator.
   - Example: Basic calculator.
     
2. Defining Task:
3. Evaluation Metric: Unit test cases
4. Initial Prompt:
   - sys_msg_code_generation = ""
   - prompt_generate_code = ""
   
6. Experiment:
   ```
   from IPython.display import Markdown
   from openai import OpenAI
   client = OpenAI()

   def get_response(prompt: str);
       response = client.chat.completions.create(
                      model="gpt-4-turbo",
                      messages=[{"role": "system", "content": sys_msg_code_genertion},
                                {"role": "system", "content": prompt}]
       )

       return response.choices[0].message.content
   python_code = get_response(prompt_Generate_code)
   Markdown(python_code)

   ```
   
