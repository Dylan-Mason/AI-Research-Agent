# AI Research Agent
LangChain AI research assistant using Google Gemini, Wikipedia & DuckDuckGo, with automatic summary saving.

# AI Research Assistant

A LangChain-powered agent that uses Google’s Gemini (via `ChatGoogleGenerativeAI`), DuckDuckGo search, and Wikipedia to fetch structured research summaries—and even saves them to a local text file automatically.

## Features

- **Multi-tool research**  
  - DuckDuckGo web searches  
  - Wikipedia API queries  
- **Structured output**  
  - Pydantic-validated JSON with `topic`, `summary`, `sources`, `tools_used`  
- **Auto-save**  
  - Appends each result to `research_output.txt` with a timestamp  
- **Easy swap of LLM**  
  - Swap in Claude, GPT-4, etc., by changing one import

## Tech Stack

- **LangChain** for orchestration and tool-calling  
- **ChatGoogleGenerativeAI** wrapper around Gemini  
- **Pydantic** for output parsing  
- **Python 3.11+**  

## Quickstart

1. Clone the repo  
2. Copy your Gemini API key into a `.env` file as `GEMENI_API_KEY`  
3. Install dependencies:  
   ```bash
   pip install -r requirements.txt
