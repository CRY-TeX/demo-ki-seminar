# Demo _Seminar Aktuelle Themen der KI_

This is a demo for the course _Seminar Aktuelle Themen der KI_, KI-B-6, TH Deggendorf for the topic "T1: Large Language Models".
We are going to leverage ChatGPT and the tool suite of [LangChain](https://python.langchain.com/en/latest/index.html) in order to build an application which would be either impossible or just with a tedious amount of work to achieve otherwise.

For this demo we are going to build a system which can do one of the subtasks for this course, creating a podcast script, fully automatically.
We will use our lecture slides to extract information about the requirements and the topic, search wikipedia and the web for current information and use this to create our podcast script.

This is done to show 3 things:

- How powerful the tool sets have become in order to automate a wide array of problems through to be impossible to solve
- The problem the educational sector faces with examination of the students
- The advantage people who have access to such tools (GPT4, ChatGPT Plugins) will have over those who don't

The second and third point are especially problematic as OpenAI is working on a [Plugins System](https://openai.com/blog/chatgpt-plugins) which will be available to the average user and will be able to more or less do the same thing shown here.

> All personal inforation in the lecture script was removed for privacy reasons.

> This demo is inspired by the work done on [Auto GPT](https://github.com/Significant-Gravitas/Auto-GPT)

## Getting Started

1. Make sure to follow all steps from the [Installation section](#installation).
2. Copy the `.env.example` file to `.env`. You need 2 API keys in order to run this demo
   - An [OpenAI API Key](https://platform.openai.com/) in order to use the API for ChatGPT
   - An [SerpApi API Key](https://serpapi.com/) in order to use the SerpApi tool
3. Now you can run the cells of the [Demo Notebook](./src/demo.ipynb) and be amazed 🥳

> Disclaimer: The SerpApi tool integration and the podcast script creation makes requests to their respective API providers. You need to have either a free account or a paid one.

## Installation

1. Make sure to have at least [Python 3.10](https://www.python.org/downloads/) installed
2. Install [Pipenv](https://pipenv.pypa.io/en/latest/) with `pip install pipenv`
3. Run `pipenv install` in the root directory of this project
