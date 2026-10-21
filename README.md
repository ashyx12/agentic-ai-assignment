# Agentic AI Assignment — Personalized Learning Assistant

A small Google Colab-first implementation of **Agentic AI-Based Personalized Learning and Student Assistance System**.

**[Open the notebook in Google Colab](https://colab.research.google.com/github/ashyx12/agentic-ai-assignment/blob/main/personalized_learning_assistant.ipynb)**

Run cells from top to bottom. The core demo uses a quiz and a simple learning-path workflow, so it does not need an API key. An optional final section downloads the small public `google/flan-t5-small` model and runs it directly in Colab to generate extra study advice—no OpenAI or Gemini API key required.

## What it does
1. Takes a learner's quiz answers.
2. Identifies topics needing revision.
3. Creates an ordered study plan with resources and practice tasks.
4. Uses three specialist components: assessor, planner, and study coach.
5. Optionally generates additional advice using a small local Hugging Face model.

The quiz and links are illustrative; replace them with your course material if necessary. The optional model needs an internet connection to download weights and benefits from a Colab GPU, but the basic workflow runs without it.
