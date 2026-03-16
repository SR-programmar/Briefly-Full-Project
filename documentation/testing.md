# Testing

```
This document shows the testing results after testing the two core parts of our software
```

**Methodology of the tests**

We created a Chrome extension called Briefly that assists the visually impaired.

We loaded Briefly into Chrome using developer mode.

The features of Briefly can be utilized by a user through keyboard commands.

We were able to record its output by logging and taking it from the console, while
some tests relied on observation and listening.

We then analyzed the output to create a final testing result.

**Chart 1 - Summarization testing**
![Summary results](graphics/sum%20test%20results.png)

**Chart 2 - AI Agent testing**
![Agent results](graphics/agent%20results.png)

## Conclusion

Briefly's main two features are

- Summarization
- Navigating using an AI Agent

Both are made possible by AI Models from OpenAI or Google

### OpenAI

- Created concise and easy-to-understand summaries
- Didn't ignore Navbar, header, and footer content
- Works well as an AI Agent

### Gemini

- Created summaries that were much better than OpenAI's summaries
- Ignored Navbar, header, and footer content
- Doesn't work well as an AI Agent because it created output that caused errors
