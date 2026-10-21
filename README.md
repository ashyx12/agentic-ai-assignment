# Multi-Agent Question-Paper Generation and Validation System

**Selected topic:** #6 from the provided project list — *Multi-Agent Question-Paper Generation and Validation System*.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ashyx12/agentic-ai-assignment/blob/main/multi_agent_question_paper.ipynb)

## Run
Open the notebook in Google Colab and run the cells from top to bottom. A GPU runtime is recommended (the 1.5B model may be slow on CPU). It downloads the small open-weight `Qwen/Qwen2.5-1.5B-Instruct` model and runs it inside Colab. **No OpenAI or Gemini API key is required.**

## Agent workflow
1. **Blueprint Agent** plans topic coverage and question types.
2. **Question Generation Agent** generates the question paper and answer key.
3. **Validation Agent** reviews relevance, ambiguity, duplicates, coverage, and answers.
4. **Revision Agent** is invoked if the validator returns `DECISION: REVISE`.

This uses a shared local language model with role-specific prompts, plus validation-driven routing and a revision loop. It is a small educational prototype: manually review generated answers before using the paper.
