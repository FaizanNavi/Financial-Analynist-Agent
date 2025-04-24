# Financial Analyst Agent

This project is a Python-based application that leverages AI agents to perform financial analysis and web searches. It uses the `phi` library and integrates tools like `YFinance` and `DuckDuckGo` to provide insights and data.

## Features

The project includes two main agents:

### 1. **Web Search Agent**
- **Purpose:** Searches the web for information.
- **Model:** `Groq` (Llama 3.3 70B Versatile).
- **Tools:** DuckDuckGo for web searches.
- **Instructions:** Always include sources in the response.
- **Output:** Markdown-formatted responses with tool call visibility.

### 2. **Financial AI Agent**
- **Purpose:** Provides financial data and analysis.
- **Model:** `Groq` (Llama 3.3 70B Versatile).
- **Tools:** 
  - `YFinanceTools` for:
    - Stock prices
    - Analyst recommendations
    - Stock fundamentals
    - Company news
- **Instructions:** Use tables to display data.
- **Output:** Markdown-formatted responses with tool call visibility.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/FaizanNavi/Financial-Analynist-Agent.git
   cd Financial-Analynist-Agent
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the following keys:
     ```plaintext
     PHI_API_KEY=<your-phi-api-key>
     GROQ_API_KEY=<your-groq-api-key>
     OPENAI_API_KEY=<your-openai-api-key>
     ```

4. Run the application:
   ```bash
   python playground.py
   ```

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

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- **Phi Library:** For providing the AI agent framework.
- **YFinance:** For financial data tools.
- **DuckDuckGo:** For web search capabilities.
