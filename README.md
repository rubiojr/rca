# Risor Code Assistant

Use AI to create Risor code.

The Risor Code Assistant is a repository containing tools, examples, and resources to enhance Large Language Models' (LLMs) ability to write Risor code. It provides context, reference implementations, and best practices to help AI models generate more accurate, efficient, and idiomatic Risor programs.

## Features

- Example Risor code snippets for common patterns
- Detailed documentation on Risor syntax and semantics
- Task-specific templates and solutions
- Debugging strategies for common Risor errors
- Performance optimization guidelines

This repository serves as a knowledge base to fine-tune AI systems to better understand and generate code in the Risor language.

## Using the context

To optimize for different token usage scenarios, we provide three versions of the Risor language context file:

- **Small context (context-small.txt)** (~2.5K tokens): Contains only essential syntax, core built-ins, and minimal examples. Best for quick coding tasks where token efficiency is critical, though may sacrifice some accuracy with advanced features.

- **Medium context (context-medium.txt)** (~3.9K tokens): Balanced approach with more comprehensive syntax coverage, common modules, and several complete examples. Recommended for most use cases as it offers a good balance between token cost and coding accuracy.

- **Large context (context-large.txt)** (~40K tokens): Complete language reference with extensive module documentation, detailed examples, and edge cases. Use when accuracy is paramount and token efficiency is less important.

Choose the context size based on your needs - smaller contexts save on token usage but may result in less accurate or idiomatic Risor code, especially for complex tasks.

> [!WARNING]
> The context-large.txt file is rather large (~40K tokens). Keep in mind that it may burn your LLM credits quite fast.

Code editors like Zed can be given a context file to provide the necessary information for the assistant to understand the problem and generate the appropriate Risor code.

https://github.com/user-attachments/assets/0bdd626e-5456-48ae-a479-7fe2feade100
