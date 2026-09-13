# Agentic RAG Lab

  A learning project from the LLM Zoomcamp exploring a basic Retrieval-Augmented Generation (RAG) workflow for answering questions about DataTalksClub courses and FAQs.

  ## Current status

  The project currently contains an experimental Jupyter Notebook that:

  - Loads the OpenAI API key from a `.env` file
  - Sends prompts to an OpenAI model
  - Builds a question-answering prompt
  - Downloads course FAQ data from DataTalksClub
  - Returns answers based on provided context

  The FAQ documents are currently downloaded into `documents`, but the `search()` function still uses hard-coded context. Retrieval using `minsearch` and more advanced agentic
  behavior are planned future improvements.

  ## Requirements

  - Python 3.11+
  - [uv](https://docs.astral.sh/uv/)
  - An OpenAI API key
  - Internet access

  ## Setup

  Install the project dependencies:

  ```bash
  uv sync
```

  Create a .env file in the project root:

  OPENAI_API_KEY=your_api_key_here

  Never commit the .env file.

  ## Running the notebook

  Start Jupyter:

```bash
  uv run jupyter lab
```
  Then open notebook.ipynb.