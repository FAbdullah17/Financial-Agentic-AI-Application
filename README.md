# Financial Agentic AI Application

This repository hosts the **Financial Agentic AI Application**, a Python-based AI system combining financial data analysis and web search capabilities. It leverages advanced AI models, financial tools, and web search utilities to provide insightful and interactive responses.

## Features

- **Financial AI Agent**:
  - Analyze stock prices, fundamentals, and analyst recommendations.
  - Retrieve the latest company news.
  - Display results using well-structured tables.

- **Web Search AI Agent**:
  - Perform web searches and provide sourced information.
  - Utilize DuckDuckGo for secure and fast searches.

- **Multi-Agent System**:
  - Combine multiple agents to create a collaborative AI.
  - Share results with sources and structured data representation.

## Prerequisites

- Python 3.8 or higher
- Environment variables for API keys:
  - `OPENAI_API_KEY` for OpenAI API access.
  - `PHI_API_KEY` for PHI API access.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/FAbdullah17/Financial-Agentic-AI-Application.git
   cd Financial-Agentic-AI-Application
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure environment variables:
   - Create a `.env` file in the root directory with the following content:
     ```
     OPENAI_API_KEY=your-openai-api-key
     PHI_API_KEY=your-phi-api-key
     ```
   - Replace the placeholders with your actual API keys.

## Usage

### Running the Financial Agent
1. Execute the script to use the financial agent and web search agent collaboratively:
   ```bash
   python main.py
   ```
2. Example prompt for the multi-agent system:
   ```plaintext
   Summarize analyst recommendations and share the latest news for NVDA.
   ```

### Running the Playground Application
1. Serve the interactive playground app:
   ```bash
   python playground_app.py
   ```
2. Access the playground interface to interact with agents.

## How It Works

1. **Agents Setup**:
   - The `Web Search Agent` uses DuckDuckGo for secure searches and includes sources in responses.
   - The `Finance AI Agent` integrates financial tools to analyze stocks and generate detailed tables.

2. **Multi-Agent Collaboration**:
   - The `multi_ai_agent` combines the strengths of both agents to provide comprehensive results.

3. **Playground Application**:
   - An interactive app built using `phi.playground` allows users to experiment with the agents.

## Dependencies

The project requires the following Python libraries:
- `phidata`
- `python-dotenv`
- `yfinance`
- `packaging`
- `duckduckgo-search`
- `fastapi`
- `uvicorn`
- `groq`
- `openai`
- `requests`

Install them using:
```bash
pip install -r requirements.txt
```

## Customization

- **Add New Tools**: Extend the agents' capabilities by adding new tools to their `tools` parameter.
- **Update Models**: Replace the `Groq` model ID with a different model if required.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Fork the repository, create a feature branch, and submit a pull request.

## Contact

For questions or support, please create an issue in the GitHub repository.
