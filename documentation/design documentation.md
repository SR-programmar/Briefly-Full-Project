# Design Documentation

This document explains how and why we designed Briefly the way we did.

Table of contents

- [Design Documentation](#design-documentation)
    - [October 23rd - November 12th, 2025](#october-23rd---november-12th-2025)
        - [Interview with two vision specialists](#interview-with-two-vision-specialists)
        - [Prototype](#prototype)
    - [November 12th, 2025 - December 5th, 2025](#november-12th-2025---december-5th-2025)
        - [Rosie, the AI Agent web assistant (version 2.0)](#rosie-the-ai-agent-web-assistant-version-20)
        - [Interview with a software engineer - November 26th, 2025](#interview-with-a-software-engineer---november-26th-2025)
        - [Interview with a previous vision specialist](#interview-with-a-previous-vision-specialist)
    - [December 5th - February 28th, 2026](#december-5th---february-28th-2026)
        - [Version 3.](#version-3)
        - [Interview with a vision specialist to test the application](#interview-with-a-vision-specialist-to-test-the-application)
        - [Version 3.](#version-3-1)
    - [Conclusion](#conclusion)
        - [One sentence Summary:](#one-sentence-summary)

## October 23rd - November 12th, 2025

### Interview with two vision specialists

We interviewed two vision specialists to define the biggest problems visually
impaired users have with technology

1. **Compatibility issues -**
   Some screen reader software was developed in the early 2000s and
   isn’t compatible with the latest versions of systems.
2. **Text-to-speech -**
   This software may not correctly read what’s on the screen.
   It’s also not pleasant to listen to its robotic-sounding voice
3. **Time consumption -**
   It takes a long time to listen to content being read aloud compared to
   reading it with your eyes
4. **Simplicity -**
   Screen reader software is very complex and hard to learn. This leads
   visually impaired users to be frustrated and neglect learning the
   software.

### Prototype

We created a prototype with the following functionality.
![prototype](graphics/how%20it%20works.png)
The prototype can summarize a webpage’s content and read it aloud.
We chose this design because:

- Summarizing a webpage’s content saves them time
- **Ctrl** is very easy to remember and located on an easy-to-find spot on your
  keyboard

## November 12th, 2025 - December 5th, 2025

### Rosie, the AI Agent web assistant (version 2.0)

Rosie is an AI Agent because it helps you perform tasks. Rosie can answer your
questions and perform more complex tasks, such as opening a website.

This helps address the problems defined because:

- the user doesn’t have to navigate using multiple keyboard commands
- The user doesn’t have to listen to irrelevant information being read aloud
  -It’s easy to learn and gets things done quickly

### Interview with a software engineer - November 26th, 2025

This software engineer reviewed our software’s code and gave us advice:

- Use Gemini instead of OpenAI
- Pre-process the webpage before handing it to AI
- Create thorough documentation

### Interview with a previous vision specialist

We had the vision specialist, one we previously interviewed, come back to test our
application. She gave us the following advice.

```
- Add sound cues during summaries and the AI Agent's responses
- Ability to pause the screen reader
- Braille instructions for Braille display or Printer embosser
```

## December 5th - February 28th, 2026

### Version 3.0

Our extension has the following capabilities:

- Summary customization
- Extension can be activated or deactivated
- AI Agent with the ability to
    - Open a website in the current tab or a new one
    - Help compose an email
    - Click buttons or links on the screen
    - Make queries on Google or YouTube
- An instructions page with printable braille instructions

All of these features can be accessed using key commands.

### Interview with a vision specialist to test the application

After incorporating all of the vision specialists' feedback, we had her come back and
test our application again to get feedback.

She recommended the following

- Send instructions to the Braille display
- English-to-Spanish translation
- Ability to set alarms
- Remove the need to ask for tab interaction

### Version 4.0

We decided to only incorporate some of the requested features before we went to
the state conference. We decided to implement Spanish translation and Gemini.

Previously mentioned, a software expert had recommended us to use Gemini
instead of OpenAI.

We upgraded our server to be able to translate English into Spanish and also use
Gemini.

## Conclusion

### One sentence Summary:

Our software assists visually impaired users on the internet by saving them time.

The three main challenges defined from the interview in October were:

- Time consumption
- Complex screen reader software
- “Robotic” sounding voices

We designed a software product that solves these problems by:

- Summarizing webpages
    - Reduces the amount of time spent listening
- Easy-to-remember and locate key commands
    - Makes it very easy to learn
- Rosie, the AI Agent
    - Saves time in performing tasks on the internet
