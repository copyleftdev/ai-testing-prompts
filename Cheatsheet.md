# OpenAI Prompt Engineering Cheat Sheet

## Overview
This cheat sheet provides guidelines and examples for crafting effective prompts to elicit the best responses from OpenAI's language models, including GPT-3 and GPT-4.

## Key Concepts

- **Prompt Engineering**: The practice of designing and refining the input given to a language model to achieve the desired output.
- **Tokens**: The pieces of text (words or parts of words) that the model processes. Effective prompt design considers token limits.
- **Temperature**: A setting that controls the randomness of the model's responses. Lower values make the output more deterministic.

## Prompting Techniques

### 1. Direct Questions
Asking direct questions tends to produce concise and specific answers.

- **Example**:
  \```plaintext
  What is the capital of France?
  \```
  **Expected Output**:
  \```plaintext
  The capital of France is Paris.
  \```

### 2. Instruction Following
Provide clear, detailed instructions for complex tasks.

- **Example**:
  \```plaintext
  Explain the theory of relativity as if I'm a ten-year-old.
  \```
  **Expected Output**:
  \```plaintext
  The theory of relativity says that the faster you move, the slower time passes for you compared to someone who is not moving.
  \```

### 3. Zero-Shot and Few-Shot Learning
Demonstrate a task with examples (few-shot) or without them (zero-shot) to guide the model.

- **Zero-Shot Example**:
  \```plaintext
  Translate 'Hello, how are you?' into French.
  \```
  **Few-Shot Example**:
  \```plaintext
  English: How are you?
  French: Comment allez-vous?
  
  English: I am fine.
  French: Je vais bien.
  
  Translate 'Where is the library?' into French.
  \```

## Advanced Prompt Design

### Contextual Embedding
Embed the task within a context to guide the model’s tone and style.

- **Example**:
  \```plaintext
  As a witty travel blogger, describe a visit to the Eiffel Tower.
  \```

### Chain of Thought
Encourage the model to "think aloud" as it approaches problem-solving tasks.

- **Example**:
  \```plaintext
  You are a detective solving a mystery. Describe your thought process as you determine who took the last cookie.
  \```

## Formatting Tips

- **Bold and Italics**: Use `**bold**` for emphasis and `*italics*` for less emphasis.
- **Lists**: Use `-` or `*` for bullet points.
- **Code**: Use backticks ` ` ` for inline code and triple backticks ``` for blocks of code.
- **Tables**:
  \```markdown
  | Task Type         | Description                         | Example Prompt                     |
  |-------------------|-------------------------------------|------------------------------------|
  | Informational     | Provides factual information.       | `What is the tallest mountain?`    |
  | Instructional     | Gives directions to perform a task. | `Describe how to bake a cake.`     |
  \```

## Best Practices

- **Be Specific**: The more specific the prompt, the more accurate and relevant the output.
- **Provide Context**: Include necessary background information to orient the model.
- **Iterative Refinement**: Start with a basic prompt, then refine based on the model's output.