LangChain Basics: Building Your First LLM Applications
This repository contains a series of Jupyter Notebooks designed to walk you through the fundamental concepts of the LangChain framework. It covers the entire workflow, from making basic Large Language Model (LLM) calls to prompt engineering, output parsing, and chaining components together to build practical applications.

🚀 Project Goal
Understand the core components of LangChain: LLMs, Prompts, and Output Parsers.

Learn to build powerful data pipelines using the LangChain Expression Language (LCEL).

Practice integrating both local models via Ollama and remote models via the OpenAI API.

Apply all learned concepts to build a multi-step mini-project.

📚 Notebooks Overview
The repository is structured as a series of hands-on labs, with each notebook focusing on a specific aspect of LangChain.

1.prompt.ipynb:

Learn to create dynamic prompts with PromptTemplate.

Practice building conversational prompts using SystemMessage, HumanMessage, and AIMessage to define roles and context.

2.output-parser.ipynb:

Use StrOutputParser to cleanly convert LLM output into a simple string.

Explore how to get structured JSON output from an LLM by combining with_structured_output with Pydantic models for predictable, easy-to-use data.

3.runnable.ipynb:

Dive into the heart of LangChain: the LangChain Expression Language (LCEL).

Practice using the pipe (|) operator to chain prompts, LLMs, and output parsers into a single, executable "Runnable" pipeline.

4.FoodChain.ipynb:

This is a capstone mini-project that combines all the concepts from the previous notebooks.

It features a primary chain that generates the name of a popular food from a given country.

A secondary chain then takes the food's name as input and generates a detailed recipe for it.

This exercise demonstrates how to create more complex, multi-step applications by linking different chains together.

🛠️ Getting Started
Follow these steps to set up the project on your local machine.

1. Clone the Repository
   bash
   git clone https://github.com/your-username/langchain-basics.git
   cd langchain-basics
2. Set Up a Virtual Environment & Install Packages
   It is highly recommended to use a virtual environment to manage dependencies.

bash

# Create a virtual environment

python -m venv .venv

# Activate the virtual environment (macOS/Linux)

source .venv/bin/activate

# Activate the virtual environment (Windows)

.venv\\Scripts\\activate

# Install the required packages

pip install -r requirements.txt 3. Configure Environment Variables
Sensitive information like API keys should be stored in a .env file. First, create a copy of the example file.

bash
cp .env.example .env
Next, open the .env file and add your OpenAI API key.

text

# .env

OPENAI_API_KEY="your_openai_api_key_here" 4. Launch Jupyter Notebook
You are now ready to run the notebooks.

bash
jupyter notebook
💡 Key Learnings
How to interface with different LLMs (both local and remote) within LangChain.

Techniques for prompt engineering to precisely control LLM responses.

Methods for parsing LLM outputs into desired data formats for downstream use.

The power of LCEL for building modular and reusable AI application chains.

💻 Technologies Used
Python
LangChain
OpenAI
Ollama
Jupyter Notebook
