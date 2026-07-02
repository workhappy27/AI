**"what is the content for ChatGPT 4.0?"**

```python
{
    "role": "system",
    "content": "???"
}
```

then the answer is **there is no single public system prompt for ChatGPT-4 or ChatGPT-4o**.

The `content` is whatever instructions the application developer provides.

For example:

```python
{
    "role": "system",
    "content": "You are a helpful assistant."
}
```

or

```python
{
    "role": "system",
    "content": "You are a senior Python developer. Give concise answers."
}
```

or

```python
{
    "role": "system",
    "content": "Answer only in JSON format."
}
```

All of these can be used with GPT-4, GPT-4o, GPT-3.5, or other chat models.

***

### In the actual ChatGPT application

OpenAI uses its own internal system instructions behind the scenes. They typically include guidance such as:

* Be helpful
* Be accurate
* Be safe
* Follow user instructions when appropriate
* Refuse harmful requests

However, the **exact system prompt used by ChatGPT is not publicly disclosed and can change over time**.

***

### Relationship between Model and Content

A common beginner misunderstanding is:

```python
model = "gpt-4o"
```

does **not** determine the content.

Instead:

```python
response = client.chat.completions.create(
    model="gpt-4o",
    messages=[
        {
            "role": "system",
            "content": "You are a helpful coding tutor."
        },
        {
            "role": "user",
            "content": "Explain recursion."
        }
    ]
)
```

* **Model** = the AI engine (GPT-4o)
* **System content** = behavior/instructions
* **User content** = task/question

Think of it like:

```text
Model  -> Brain
System -> Personality and rules
User   -> Question
```

The same GPT-4o model can act as a teacher, doctor, translator, interviewer, code reviewer, or travel guide simply by changing the `system` message content.
