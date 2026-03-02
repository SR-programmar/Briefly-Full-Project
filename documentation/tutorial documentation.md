# Tutorial Documentation

```
This document teaches you how to use Briefly.
```

Table of Contents

- [Tutorial Documentation](#tutorial-documentation)
  - [Introduction](#introduction)
    - [Use Case](#use-case)
    - [Target Users](#target-users)
    - [Main Features](#main-features)
  - [System Architecture](#system-architecture)
    - [Flowchart Labels:](#flowchart-labels)
  - [Features](#features)
    - [Summarizer](#summarizer)
    - [A.I Agent](#ai-agent)
  - [User Guide](#user-guide)
    - [Installation:](#installation)
    - [Key commands overview](#key-commands-overview)
    - [Summarization](#summarization)
    - [Commands when summarization is idle](#commands-when-summarization-is-idle)
    - [Agent Commands](#agent-commands)
    - [Briefly Key Command Tutorial](#briefly-key-command-tutorial)

## Introduction

### Use Case

Briefly helps visually impaired users navigate the internet by
saving them time.

### Target Users

This program is intended for any blind and low-vision users
who rely on a screen reader.

### Main Features

The main features of this program are as follows:

- Summarizer

- Summarizes text content on the current page
- Has different options like long, short, 2-sentences
  -A.I Agent
- Helps navigate through the browser and pages
- E.g., openURL, listTabs, clickElement

## System Architecture

![System Architecture](graphics/AI%20Agent%20architecture.png)

### Flowchart Labels:

```
-Blue Box: Process - A function/action
-Diamond: Decision - A yes/or no outcome
-Pink Box: Input for the process
-Purple Box: Output for the process
```

## Features

### Summarizer

```
-Uses Artificial intelligence to summarize an entire
webpage
-Its length can be modified to be Long, Medium, Short, or
two-sentence
-The type of summary can be customized
```

### A.I Agent

```
-Overview: The A.I agent uses a Natural Language
Processor from OpenAI to process user input and choose
the best function for it based on its predefined functions.
-Functions:
```

1. **Answer:** The A.I Agent will answer the user’s question, just like
   Siri or Google, when the user doesn’t ask for a function.
2. **listTabs():** The A.I Agent will tell the title of all the tabs that are
   currently open.
3. **openURL():** The A.I Agent will open the specified website the
   user asks for in a new tab.
4. **clickElement():** The A.I Agent will search for an interactive
   element (e.g. buttons, anchors) with a specific text content and click
   on the element that matches the input. (E.g. On YouTube,
   clickElement(“Moana”) would search for a video titled Moana and click
   on it)

## User Guide

```
Note: This is a summary of the user guide. The complete
user guide will be present when you install the extension.
```

### Installation:

The extension is not available on the Chrome Web Store. You
may download through Github but this is primarily a strategy
for developers.

```
-Step 1: Download the extension fromGithub
-Step 2: Go to chrome://extensions
-Step 3: Enable Developer Mode & Load Extension File
```

### Key commands overview

**3x -** This means you must press the key 3 times

**Activation**

- Shift + Ctrl to activate or deactivate it
- Shift 3x - Instructions page with braille printable instructions

### Summarization

- Ctrl 3x - Webpage is summarized and read aloud
- Ctrl - Cancel
- Capslock - Pause

### Commands when summarization is idle

- Shift - Change Length
- Capslock - change summary type

### Agent Commands

- Hold F2 (1+ second) - Activate Agent
- ESC - Terminate conversation
- Ctrl - Interrupt it
- Capslock - Pause

### Briefly Key Command Tutorial

**Activation**

**User gesture -** You need to interact with the webpage with
your keyboard or mouse for the key commands to work.
Pressing Shift + Ctrl will notify you if you haven’t already
done this. More aboutuser activation.

**Shift + Ctrl -** Activates or deactivates the extension

**Summarization commands**

- **Ctrl 3x times** - You will get a summary of the page read out loud.
- **Ctrl** - If the screen reader is actively speaking, it is
  cancelled
- **Capslock** - If the screen reader is active, it is paused and can be resumed if capslock is pressed again

**Summarization customization**<br>
The screen reader must not be actively speaking
the summary for these commands to work

- **Shift** - Cycles through the different summary
  lengths: Long, medium, Short, and Two-sentence
- **Capslock** - Cycles through the different summary
  types: General, Paragraph, Learn, and Research

**A.I Agent Commands**

- **Hold down F2 for at least 1 second** - Initiates
  conversation with Rosie. Tell Rosie your questions or what you want to happen in
  your browser
- **Ctrl** - Interrupts Rosie, which switches her into listening
- **Esc**- Terminates the conversation
