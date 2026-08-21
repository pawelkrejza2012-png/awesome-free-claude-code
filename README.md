# awesome-free-claude-code
# Awesome Free Claude Code & AI CLI Workarounds 🚀

A curated list of free methods, alternative API endpoints, and local setups to run Anthropic's Claude Code CLI and other AI developer tools completely for free. 

---

## 🔥 Free API Endpoints & Proxies

* **[Google AI Studio](https://aistudio.google.com)** - Get a 100% free API key for Gemini models with massive rate limits and no credit card required.
* **[OpenRouter Free Models](https://openrouter.ai)** - Access free hosted models (Llama 3, Qwen, Mistral) through a unified OpenAI-compatible API link.
* **[Groq Cloud](https://groq.com)** - Extremely fast open-source models with a generous free tier for developers.

## 💻 Local Offline Setups (No API Keys)

* **[Ollama](https://ollama.com)** - Run powerful coding models (DeepSeek-Coder, Llama3, Codegemma) directly on your own GPU/CPU hardware.
* **[LM Studio](https://lmstudio.ai)** - A desktop application to discover, download, and run local LLMs with a built-in local server setup.

---
## 🛠️ Configuration Guides

### Windows (Command Prompt - CMD)
To redirect your Claude Code CLI to a free API, open your command prompt and run these variables before executing the `claude` command:

```cmd
set ANTHROPIC_BASE_URL=https://openrouter.ai/api/v1
set ANTHROPIC_API_KEY=YOUR_FREE_OPENROUTER_KEY
set ANTHROPIC_MODEL=meta-llama/llama-3-8b-instruct:free
claude
```

### macOS & Linux (Bash / Zsh)
Open your terminal and run the following export commands before launching the CLI:

```bash
export ANTHROPIC_BASE_URL="https://openrouter.ai/api/v1"
export ANTHROPIC_API_KEY="YOUR_FREE_OPENROUTER_KEY"
export ANTHROPIC_MODEL="meta-llama/llama-3-8b-instruct:free"
claude
```

## 📊 Recommended Free Coding Models

| Provider / Model Name | OpenRouter Model Slug | Context Window | Best For |
| :--- | :--- | :--- | :--- |
| **OpenRouter (Auto)** | `openrouter/free` | 200k | Automatically routes to the best available free model |
| **Meta (Muse Spark)** | `meta/muse-spark-1.2:free` | 1M | Massively long code context & multi-file refactoring |
| **NVIDIA (Nemotron Ultra)** | `nvidia/nemotron-3-ultra:free` | 1M | Deep logic, architecture design & fast code outputs |
| **Cohere (North Mini Code)** | `cohere/north-mini-code:free` | 256k | Specialized, lightweight software engineering tasks |
| **Google (Gemma 4)** | `google/gemma-4-26b-a4b:free` | 256k | Clean scripts, function calling & structured JSON data |

*Contributions, suggestions, and stars are highly appreciated! Let's build the ultimate resource for free AI coding tools together.*
