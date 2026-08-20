# awesome-free-claude-code
# Awesome Free Claude Code & AI CLI Workarounds 🚀

A curated list of free methods, alternative API endpoints, and local setups to run Anthropic's Claude Code CLI and other AI developer tools completely for free. 

---

## 🔥 Free API Endpoints & Proxies

* **[Google AI Studio](https://google.com)** - Get a 100% free API key for Gemini 2.5 models with massive rate limits and no credit card required.
* **[OpenRouter Free Models](https://openrouter.ai)** - Access free hosted models (Llama 3, Qwen, Mistral) through a unified OpenAI-compatible API link.
* **[Groq Cloud](https://groq.com)** - Extremely fast open-source models with a generous free tier for developers.

## 💻 Local Offline Setups (No API Keys)

* **[Ollama](https://ollama.com)** - Run powerful coding models (DeepSeek-Coder, Llama3, Codegemma) directly on your own GPU/CPU hardware.
* **[LM Studio](https://lmstudio.ai)** - A desktop application to discover, download, and run local LLMs with a built-in local server setup.

## 🛠️ Configuration Guide for Windows (CMD)

To redirect your Claude Code CLI to a free API, open your command prompt and run these variables before executing the `claude` command:

```cmd
set ANTHROPIC_BASE_URL=https://openrouter.aiapi/v1
set ANTHROPIC_API_KEY=YOUR_FREE_OPENROUTER_KEY
set ANTHROPIC_MODEL=meta-llama/llama-3-8b-instruct:free
claude
```

---
*Contributions, suggestions, and stars are highly appreciated! Let's build the ultimate resource for free AI coding tools together.*
