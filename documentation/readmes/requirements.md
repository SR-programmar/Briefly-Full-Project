# Requirements Documentation

This document describes the software’s functionality, features, and
how it should perform<br>

<br>

**Briefly** is a Chrome extension that is an add-on to the Chrome
browser to provide additional features for the visually impaired.
The software can summarize webpages with artificial intelligence
and then read those summaries aloud with a tool called **screen
reader** , which translates text into audio.<br>

Briefly also has an AI agent, named **Rosie** , that helps a user
navigate through the internet. Rosie provides aid to the visually
impaired as if there is a person by their side to help them navigate
through the browser.<br>

## Functional Requirements

**Extension Activation (Shift + Ctrl) -** If the user presses Shift +
Ctrl, then the extension should be activated; if the extension is
already active and the user presses this keyboard command, then
the extension should be deactivated.<br><br>
**Summarization (Ctrl x3)** - When the user presses Control 3 times,
the webpage should be summarized and read aloud by a screen
reader.<br><br>
**Cancel Summary (Ctrl) -** If the user presses the control key while
the screen reader is reading the summary, then the screen reader
will stop.<br><br>
**Pause Screen reader (Capslock) -** If the user presses Capslock
while the screen reader is active, then the screen reader will be
paused. If the user presses capslock when the screen reader is
paused, it will unpause and resume.<br><br>
**Change Summary type (Capslock) -** If the user presses Capslock
when the screen reader isn’t active at all, then the **type** of
summary will change, and the user will be notified of what they
selected.<br><br>

**Change Summary Length (Shift) -** If the user presses Shift while
the screen reader and AI Agent are inactive, then a new length for
the summary will be chosen, and the user will be alerted.<br><br>
**Start Agent Conversation (F2 1+ second) -** If the user holds down
F2 for 1 second, a conversation with the AI Agent will initiate. The
user and AI Agent will speak back and forth until the escape key is
pressed, terminating the conversation.<br><br>
**Interrupt AI Agent (Ctrl) -** If the user presses Ctrl while the AI
Agent is active, then the AI Agent will be interrupted and continue
listening to audio input from the user’s microphone.<br><br>
**End Agent Conversation (Esc) -** If a conversation with the AI Agent
is ongoing, then pressing escape will end the conversation.<br><br>
**Toggle language (`) -** If the user presses back tick on their
keyboard, then the language of the screen reader will be toggled
between Spanish and English.<br><br>

### Update state across all tabs

If the extension or AI Agent becomes active, then every tab in the
user’s session should update its local variables to match the
current state of the extension and AI Agent.

## Non-functional requirements

### Easy-to-learn Keyboard commands

The keyboard commands should be easy to remember and locate
on a keyboard through touch.

### Pleasant screen reader voice

The screen reader’s voice shouldn’t sound robotic but more
human-sounding; the screen reader’s voice should be pleasant to
listen to.

### Grant Permission only once

The user should grant Briefly permission to listen from their
microphone; they should only have to do this once instead of
multiple times.

### Maximum conversation time

The user is allowed only a maximum of 15 seconds to chat with
Rosie before she sends a response.
If a conversation is started and no audio input is heard for at least
10 seconds, the AI Agent will cancel itself.

### Error handling

If an error occurs from the back-end server, then the front-end
software will catch it and alert the user to what happened and log

the error in the console for developers. The program will resume
execution and continue to work.
