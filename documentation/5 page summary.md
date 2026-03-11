# Project Briefly - 1 Page summary

## 1. How it works (visual representation)

![prototype](graphics/how%20it%20works.png)

## 2. The journey

**Oct 23rd - Nov 12th, 2025** - Defined the biggest challenges and created a

prototype

**Nov 12th - Dec 5th, 2025** - Created Rosie, the AI Agent web assistant, and gained

feedback from experts.

**Dec 5th - Feb 28th, 2026** - Incorporated all feedback, adding customization,

strengthening Rosie, and utilizing **Google’s Gemini**

**Feb 28th, 2026 - March 19th, 2026** - Fixed any remaining errors, prepared

documentation, and project repository for submission

## 3. How it works

**Front-end (Chrome extension) -** Sends necessary information to the Python

server. It listens for input from the user's microphone and registers triggered

keyboard commands.

**Back-end (Python server) -** Makes API calls to Gemini or OpenAI, sending it user prompts and

pre-processed webpage content

**The Brain (Gemini) -** Performs the summarization of webpages

## 4. Quality of the software’s functionality

We loaded the Briefly Chrome extension into Chrome and logged all responses given by
Artificial Intelligence to evaluate the software.

```
● Summaries were concise and easy to understand.
● Gemini understood how to customize summaries, but sometimes returned
massive output.
● Gemini was superior to OpenAI but sometimes returned unusable output
that caused errors.
```

# Project Briefly - 4 Page summary

# Project Timeline

```
Time Frame | Milestone | Activites
```

### Oct - Nov 12th, 2025 - Foundation and Prototype

**Interview**

```
Time consumption and complex screen reader
software are the biggest challenges faced by
visually impaired users who use a computer.
```

**Prototype**

```
Press Ctrl 3x to summarize a webpage with
OpenAI.
```

### Nov - Dec 5th - Rosie and expert feedback

**Introducing Rosie!**

```
Can answer questions and navigate to websites
```

**Interview with a software engineer**

```
Recommended pre-processing and switching to
Gemini
```

**Interview with a previous vision specialist**

```
She suggested sound cues during summarization
and the ability to pause the screen reader.
```

### Dec - Feb 28th, 2026 - Customization, stronger Rosie, and Gemini

**Summarization Customization**

```
Summary can be customized in length, type, or
language
```

**Stronger Rosie**

```
She can now help compose an email and click
elements on the screen
```

**Gemini**

```
The server makes API calls to Gemini for better
summaries, but still uses OpenAI to act as Rosie.
```

### Feb - Mar 19th Software Finalization Debugging, documentation, and a repository.

```
Before the conference, we created a repository with both the back and front
ends of Briefly, and the software was thoroughly
tested to ensure no ill performance.
```

# Briefly Design

From an interview in October with two vision specialists, we collected information

on the 3 biggest challenges. We designed our software to address each challenge.

```
Challenge | Solution and Design
```

## Time Consumption

**Summary**

```
Briefly can summarize a webpage with Artificial
Intelligence, to provide only the relevant or wanted
information.
```

**Rosie**

```
Our AI Agent can answer questions directly and can
help perform common tasks on the web that would
be difficult to perform with a common screen reader.
```

## Complex Screen reader software

```
All of Briefly’s keyboard commands typically involve
one key and are all located on the left side of the
keyboard, making them easy to learn and locate.
```

## Robotic-sounding voices

```
A screen reader’s voice doesn’t sound human at all.
We chose a voice that is very pleasant to listen to.
```

# How Briefly Works

![Briefly architecture](graphics/5%20page%20sum/briefly%20structure.png)
**Frontend**

The front-end of Briefly listens to input from the keyboard or the user's

microphone. It can communicate with the user by translating text into audio. It

sends webpage content and user prompts to the back-end.

**Backend**

The back-end scrubs the webpage of unwanted text. It instructs Artificial

Intelligence on how to behave and then feeds it the cleaned content. The AI

generates a result and sends it back to the backend, which then forwards it to the

frontend.

**Gemini**

Gemini is the AI Model that’s instructed to summarize content

**OpenAI**

A model from OpenAI is what pretends to be "Rosie"

# Testing

Methodology

```
● We created the software and loaded it into Chrome using developer mode
● We logged and took output from the console to make evaluations
```

**Summarization testing**

![Summary results](graphics/sum%20test%20results.png)

**AI Agent testing**

![Agent results](graphics/agent%20results.png)

# Citations

Websites and Software

● [Canva](https://www.canva.com/)<br>
● [Lucid Chart](https://www.lucidchart.com/pages)

Icons and Graphics

● [Chrome Icon](https://www.flaticon.com/free-icon/chrome_6125000?term=chrome&page=1&position=1&origin=search&related_id=6125000)<br>
● [Server](https://www.flaticon.com/free-icon/server_4227991?term=server&page=1&position=8&origin=search&related_id=4227991)<br>
● [Artificial Intelligence Icon](https://www.flaticon.com/free-icon/artifical-intelligence_12383811?term=artifical%20intelligence&page=1&position=12&origin=search&related_id=12383811)
