# 🧭 Leadership Mentor Agent

A simple yet functional AI agent that acts as a leadership mentor, built in under 200 lines of Python. This project shows how to combine LLMs with structured tools, memory, and goal-driven logic to create a real agentic experience.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rafapaez/Leadership-Mentor-Agent/blob/main/Leadership_Mentor_Agent.ipynb)

## 🧠 What It Does

This agent simulates a leadership mentor. It can:

- Clarify your leadership goal
- Teach core leadership concepts
- Evaluate your understanding
- Guide you toward action
- End the session when appropriate

It runs in an interactive loop using the `litellm` library and is optimized for Google Colab.

## 📦 How to Use

1. **Open in Google Colab** using the badge above.
2. Go to the left sidebar → **Secrets tab** → add your OpenAI key as `OPENAI_API_KEY`.
3. Run each cell top to bottom.
4. At the end, you'll be asked:  
   _"What leadership goal would you like to work on today?"_
5. Interact with the agent directly through the console.

No setup needed. No extra dependencies beyond `litellm`.

## 🔍 Behind the Scenes

The agent follows a simple 6-step loop:

1. Construct the full prompt
2. Query the LLM
3. Parse the response (JSON with tool + arguments)
4. Execute the selected tool (clarify, teach, evaluate, finish)
5. Capture user feedback
6. Decide whether to continue or end

Tools are defined as Python functions and selected by the LLM based on the conversation.

## 📖 Read the Full Breakdown

Read the full write-up on [The Engineering Leader]([https://newsletter.rafapaez.com/](https://open.substack.com/pub/rafapaez/p/build-your-first-ai-agent)).

## ✨ Future Improvements

- Add long-term memory across sessions
- Connect to a leadership knowledge base
- Expose as a Slack bot or web app
- Add more tools (plan, reflect, give feedback)

## 🤝 License

MIT License. Feel free to fork, remix, or build on top.
