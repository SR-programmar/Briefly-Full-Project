# Code Documentation

```
This document details how the code works for Briefly, an app designed to assist the
visually impaired.
```

## Table of contents

- [Summarization](#summarization)<br>
- [AI Agent](#ai-agent-rosie)<br>
- [Conclusion](#conclusion)

## Introduction

There are some facts about Briefly that you need to know to understand the rest of
the documentation.

Briefly consists of two parts<br>
● **The front-end** - The Chrome extension programmed in JavaScript<br>
● **The back-end** - A server programmed in Python

## Summarization

Our extension can summarize the current webpage’s content and then read it
aloud. Here is the process:

![Process](../graphics/code%20doc/summarization%20process.png)
Our **front-end** sends the webpage to the **back-end** , which then pre-processes it.

The **back-end** makes API calls to Artificial Intelligence from **OpenAI** or **Gemini**

The AI summarizes the content, and the summary makes its way back to the
**front-end.**

## AI Agent Rosie

The AI Agent’s process of analysis works very similarly to summarization.

**Front-end → Back-end → AI <br>
AI→ Back-end → Front-End**

Two major differences

- The agent expects a user prompt
- The agent returns a JSON object

The **JSON object** is processed at the **front-end** , resulting in a response and/or an
operation.

**Example JSON Object**

    {

    "agentResponse": “Sure, opening YouTube in the

    current tab”,

    "index": 1,

    "arguments": {url: “https://www.youtube.com/”}

    }

Here’s the purpose of each parameter.
![Purpose](../graphics/code%20doc/purpose.png)
The **index** for a function is the browser operation that needs to be performed. An
**index** of -1 means no operation is required.

## Testing

**Methodology of the tests**

We created a Chrome extension called Briefly that assists the visually impaired.

We loaded Briefly into Chrome using developer mode.

The features of Briefly can be utilized by a user through keyboard commands.

We were able to record its output by logging and taking it from the console, while
some tests relied on observation and listening.

We then analyzed the output to create a final testing result.

**Chart 1 - Summarization testing**
![Summary results](../graphics/sum%20test%20results.png)

**Chart 2 - AI Agent testing**
![Agent results](../graphics/agent%20results.png)

## Conclusion

Briefly consists of two parts

- Front-end (Chrome Extension)
- Back-end (Python Server)

Briefly relies on NLPs from **OpenAI or Google**

The core features of our extension are

- Summarization
- An AI Agent Web assistant
