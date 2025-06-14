# AI-agent

## Overview

AI-agent is a modular, multi-agent project for developing, testing, and benchmarking AI agents. It features both simple and advanced agent implementations in Python, with a structure that supports future expansion to other languages. The project is organized for easy experimentation, extension, and integration with external AI tools and APIs.

## Features
- **Simple Agents:** Lightweight agents using LangChain, LangGraph, and MCP for tool integration and LLM orchestration. They can scrape, crawl, and extract data from the web using Firecrawl tools and support both Mistral and Gemini models.
- **Advanced Agents:** More sophisticated agents with modular workflows, custom prompts, and structured output using Pydantic models. They focus on developer tool research, company analysis, and workflow automation.
- **Extensible Architecture:** Easily add new agents, workflows, or models. Each agent is self-contained, with clear separation between simple and advanced logic.
- **Ready for Research and Prototyping:** Ideal for rapid prototyping, benchmarking, and educational purposes.

## Project Structure

- `advanced-agent/` – Advanced AI agent implementation in Python.
  - `main.py` – Entry point for the advanced agent (to be implemented).
  - `src/` – Source code for advanced agent logic:
    - `firecrawl.py` – Firecrawl API integration for web scraping and search.
    - `models.py` – Pydantic models for structured company and tool analysis.
    - `prompts.py` – Custom prompts for LLM-driven research and extraction.
    - `workflow.py` – Workflow orchestration using LangGraph and Google Gemini.
  - `pyproject.toml`, `uv.lock` – Python project configuration and dependencies.
- `advanced-ai-agent/` – Alternative advanced agent implementation (mirrors advanced-agent structure).
- `simple-agent/` – Simple AI agent in Python.
  - `main.py` – Entry point for the simple agent, using LangChain, MCP, and Firecrawl tools.
- `simple-ai-agent/` – Alternative simple agent implementation (mirrors simple-agent structure).
- `README.md` – Project documentation.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ai-agent.git
   cd ai-agent
   ```
2. **Install dependencies:**
   Each agent has its own dependencies. For Python agents:
   ```bash
   cd advanced-agent
   pip install -r requirements.txt  # or use pyproject.toml with poetry/uv
   ```
   Repeat for other agent directories as needed.
3. **Set up environment variables:**
   - Create a `.env` file in each agent directory and add your API keys (e.g., `MISTRAL_API_KEY`, `FIRECRAWL_API_KEY`).
4. **Run an agent:**
   ```bash
   python main.py
   ```

## Contributing

Contributions are welcome! Please open issues or pull requests for new features, bug fixes, or documentation improvements.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Inspired by open-source AI agent frameworks and research.
- Thanks to all contributors and the open-source community.
