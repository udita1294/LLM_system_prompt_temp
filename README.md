#  System Prompts

This repository contains my learning notes and code while exploring **Prompt Engineering** using the **Groq API** and **Llama 3.3 70B Versatile** model.

The objective of this exercise was to understand how **System Prompts** influence the behavior of a Large Language Model (LLM).

---

## Learning Objective

In this lesson, I learned how to:

- Connect to the Groq API using Python
- Use environment variables to securely store API keys
- Create chat completion requests
- Understand the difference between **System Prompt** and **User Prompt**
- Control the model's creativity using the **temperature** parameter

---

##  Concepts Covered

### System Prompt

A **System Prompt** defines the role or behavior of the AI before it processes the user's request.

Example:

```python
message_system = {
    "role": "system",
    "content": "You are a brand manager who suggests names for a new food brand. The name should be in one word and catchy."
}
```

---

### User Prompt

The user prompt contains the actual instruction.

```python
message = {
    "role": "user",
    "content": "Suggest me one names for a new food company."
}
```

---

### Temperature

The `temperature` parameter controls how creative or random the model's responses are.

```python
temperature = 1
```

| Temperature | Behavior |
|------------|----------|
| 0.0 | More deterministic |
| 0.5 | Balanced |
| 1.0 | Creative |
| 2.0 | Highly random |

---

## ⚙️ Technologies Used

- Python
- Groq Python SDK
- python-dotenv
- uv

---

##  Folder Structure

```text
day2/
│
├── hello_llm.py
├── .env
├── .gitignore
├── pyproject.toml
├── uv.lock
└── README.md
```

##  Key Takeaways

- Learned the purpose of **System Prompts**
- Understood how chat messages are structured
- Explored prompt engineering fundamentals
- Learned how temperature affects LLM outputs
- Practiced using the Groq Chat Completion API

---
