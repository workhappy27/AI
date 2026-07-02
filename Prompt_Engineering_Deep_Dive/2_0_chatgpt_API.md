

```
from openai import OpenAI

client = OpenAI()

def get_response(prompt_question):
    response = client.chat.completions.create(
        model="gpt-3.5-turbo-0125",
        messages=[
            {
                "role": "system",
                "content": "You are a helpful research and programming assistant"
            },
            {
                "role": "user",
                "content": prompt_question
            }
        ]
    )

    return response.choices[0].message.content

print(get_response("What is the capital of France?"))

```
This example is not really about finding the capital of France. The **capital of France** is just a very simple test question. The real purpose of the example is to teach **how prompts are sent to an LLM and how different prompt components influence the model's behavior**.

Let's break it down.

## What the code is trying to show

The tutorial is using the Chat Completion API:

```python
response = client.chat.completions.create(
    model="gpt-3.5-turbo-0125",
    messages=[
        {"role": "system",
         "content": "You are a helpful research and programming assistant"},
        {"role": "user",
         "content": prompt_question}
    ]
)
```

Conceptually, the model receives:

### System Message

```text
You are a helpful research and programming assistant
```

This defines the AI's role, personality, expertise, and behavior.

### User Message

```text
What is the capital of France?
```

This is the actual task or question.

The model then generates an assistant response such as:

```text
The capital of France is Paris.
```

***

## Why "What is the capital of France?" is commonly used

In prompt engineering tutorials, instructors often use extremely simple questions because:

### 1. The answer is known

Everyone knows the correct answer.

```text
Question: What is the capital of France?
Answer: Paris
```

So you can focus on **prompt behavior**, not on whether the model knows the facts.

***

### 2. Easy to observe prompt changes

Suppose you change the system prompt:

#### Example 1

```python
{"role":"system",
 "content":"Answer in one word only"}
```

Output:

```text
Paris
```

#### Example 2

```python
{"role":"system",
 "content":"Answer like a pirate"}
```

Output:

```text
Ahoy! The capital of France be Paris!
```

#### Example 3

```python
{"role":"system",
 "content":"Answer as a geography professor"}
```

Output:

```text
The capital city of France is Paris, which serves as the country's political, cultural, and economic center.
```

The question stays the same, but the **prompt changes the response style**.

This is exactly what prompt engineering studies.

***

## What prompt engineering is teaching here

Prompt engineering is about controlling:

### Role

```python
{"role":"system",
 "content":"You are an experienced data scientist"}
```

### Format

```python
{"role":"system",
 "content":"Always respond in JSON"}
```

### Tone

```python
{"role":"system",
 "content":"Respond formally"}
```

### Constraints

```python
{"role":"system",
 "content":"Limit response to 20 words"}
```

### Reasoning

```python
{"role":"system",
 "content":"Explain step-by-step"}
```

The France example lets you see these effects clearly.

***


## Key takeaway

The tutorial is **not teaching geography**. It is teaching the structure of a prompt:

```text
System Prompt  -> Defines behavior
User Prompt    -> Defines task
Model Output   -> Generated response
```

Using a simple question like *"What is the capital of France?"* removes all complexity so learners can clearly observe how different prompting techniques (role prompting, instruction prompting, formatting constraints, chain-of-thought prompts, etc.) affect the model's output.
