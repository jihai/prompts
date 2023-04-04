# productive-ai-prompts
This repository serves as a comprehensive list of productivity-focused prompts and prompt engineering tips that I have discovered or created.

# Tips on prompt engineering
As I continue to learn, these tips may be refined over time:

1. Role is important: GPT-4 API allows you to define a role in a separate section.
   - Role example: You are an expert engineer explaining the following code to an entry-level engineer. Please provide a step-by-step explanation of what the code does and how it works.
2. Zero-shot or Few-shot: In my experience, few-shot prompts with examples often perform slightly better. This is consistent with the "Show and Tell" and "Provide Quality Data" principles.
   - Examples are especially useful when incorrect information is not tolerated. For instance:
   ```
    Q: Who is Batman?
    A: Batman is a fictional comic book character.

    Q: What is torsalplexity?
    A: ?

    Q: What is Devz9?
    A: ?
   ```
3. Provide more details: Include additional information, such as the API to be used or any relevant input parameters required to run the code, for better results.
4. Use a suffix and edit mode?

Some useful resources I found online include:
- [best-practices-for-prompt-engineering-with-openai-api](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api)
- [prompt-design](https://platform.openai.com/docs/guides/completion/prompt-design)

# GPT4 Prompts
### Code2NL (explain this code)
```
Instructions:
You are an expert engineer who is explaining the below code to someone who is entry level engineer. Please provide a step-by-step explanation of what the code does and how it works.

Code:
"""
{clipboard}code...
"""
Your answer:
```
### NL2Code (Implement this using Python/Rust/...)
```
As an expert engineer in the software industry, you are helpful, friendly, creative, and clever. You always provide detailed step-by-step instructions for implementation.

My Request: ...
(E.g, You want to create a Python script that shows the current weather in a specific city. Please write a code that accepts the city name as input and returns the current weather information in a format that you prefer. The weather information should include temperature, humidity, wind speed, and weather condition (e.g., cloudy, sunny, etc.). Your code should use a weather API of your choice and handle potential errors.)


Your Answer: 
```

# Productivity Tips
I have been experimenting with Raycast, Zed, and Warp recently. Those new products are truly amazing.
## Generating CLI Prompts (Terminal Experience)

Warp AI outperforms GitHub Copilot CLI, as the suggested CLI commands often have issues or require additional input. Copilot's approach, which only runs or cancels the suggested command, can be problematic.
## Writing GPT4 Prompts
Right prompt templates can save lots of time. One way to achieve that is through launcher app.
1. Launcher: Raycast, when combined with snippets, extensions, and AI features, surpasses Alfred. Snippets can be used to assemble the final prompt for GPT-4 with just a few keystrokes, which is impressive (example snippets can be found [here](raycast/raycast-snippets.json)). 
