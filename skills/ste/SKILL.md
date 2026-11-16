---
name: ste
description: Write explanations in ASD-STE100 Simplified Technical English (short sentences, simple words, one idea per sentence). Use this whenever you explain something to the user in conversation, for example "how does X work", "why did Y fail", "what is the difference between A and B", "explain this code or error", "walk me through the plan", or a summary of what you changed and why. Do not use it for code, commit messages, file contents, or short replies that explain nothing.
---

# Simplified Technical English

Use ASD-STE100 rules when you explain something in conversation. The goal is text that is clear, short, and has one meaning.

## When to use

Use this skill when the reply must make the user understand something. The reader must learn the logic: what happens, why it happens, and when it matters.

Use it for these replies:

- "How does the auth flow work?"
- "Why did the build fail?"
- "What is the difference between a mutex and a semaphore?"
- "Explain this error" or "Explain this function."
- A summary of a change: what you did, why, and what the user must do next.

Do not use it for these items:

- Code, config, commit messages, or text that goes into a file.
- A short reply, such as "Done" or a one-line answer.
- Text where the user asks for a different style.

## How to explain

1. Start with the answer in one or two sentences.
2. Explain the logic. Tell the steps in the order that they occur.
3. Tell the user when to use it, or when it is important.
4. Give one small example if the idea is abstract.

## Rules

1. Write short sentences. Use a maximum of 20 words in each sentence.
2. Write one idea in each sentence.
3. Write short paragraphs. Use a maximum of 6 sentences in each paragraph.
4. Use simple, common words. Use "use", not "utilize". Use "help", not "facilitate".
5. Give one word one meaning. When you use a word for a thing, use the same word each time.
6. Use the active voice. Write "The server sends the file", not "The file is sent".
7. Use simple tenses: present, past, and future.
8. Keep "a", "an", and "the" in sentences.
9. Do not make long groups of nouns. Write "the speed of the engine", not "engine speed control unit setting".
10. For steps, use commands. Write one step in each sentence, for example "Open the file."
11. Put the most important information first.
12. Use a list when you have more than two items or steps.

## Example

Question: "Why do we cache this?"

Not STE:

> In order to facilitate the efficient utilization of resources, caching is leveraged so that redundant database round-trips are minimized.

STE:

> The cache keeps a copy of the result. When the same request comes again, the app reads the copy. It does not ask the database again. This makes the page faster. Use a cache when the data does not change often.
