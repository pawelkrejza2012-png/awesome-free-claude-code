# awesome-free-claude-code
# Awesome Free Claude Code & AI CLI Workarounds 🚀

A curated list of free methods, alternative API endpoints, and local setups to run Anthropic's Claude Code CLI, OpenAI Codex, and other AI developer tools completely for free. 

---

## 🔥 Free API Endpoints & Proxies

* **[Google AI Studio](https://google.com)** - Get a 100% free API key for Gemini models with massive rate limits and no credit card required.
* **[OpenRouter Free Models](https://openrouter.ai)** - Access free hosted models (Llama 3, Qwen, Mistral) through a unified OpenAI-compatible API link.
* **[Groq Cloud](https://groq.com)** - Extremely fast open-source models with a generous free tier for developers.

## 💻 Local Offline Setups (No API Keys)

* **[Ollama](https://ollama.com)** - Run powerful coding models (DeepSeek-Coder, Llama3, Codegemma) directly on your own GPU/CPU hardware.
* **[LM Studio](https://lmstudio.ai)** - A desktop application to discover, download, and run local LLMs with a built-in local server setup.

---

## 📊 Recommended Free Coding Models

| Provider / Model Name | OpenRouter Model Slug | Context Window | Best For |
| :--- | :--- | :--- | :--- |
| **OpenRouter (Auto)** | `openrouter/free` | 200k | Automatically routes to the best available free model |
| **Meta (Muse Spark)** | `meta/muse-spark-1.2:free` | 1M | Massively long code context & multi-file refactoring |
| **NVIDIA (Nemotron Ultra)** | `nvidia/nemotron-3-ultra:free` | 1M | Deep logic, architecture design & fast code outputs |
| **Cohere (North Mini Code)** | `cohere/north-mini-code:free` | 256k | Specialized, lightweight software engineering tasks |
| **Google (Gemma 4)** | `google/gemma-4-26b-a4b:free` | 256k | Clean scripts, function calling & structured JSON data |

---

## 🛠️ Configuration Guides

### Windows (Command Prompt - CMD)
To redirect your Claude Code CLI to a free API, open your command prompt and run these variables before executing the `claude` command:

```cmd
set ANTHROPIC_BASE_URL=https://openrouter.ai
set ANTHROPIC_API_KEY=YOUR_FREE_OPENROUTER_KEY
set ANTHROPIC_MODEL=openrouter/free
claude
```

### macOS & Linux (Bash / Zsh)
Open your terminal and run the following export commands before launching the CLI:

```bash
export ANTHROPIC_BASE_URL="https://openrouter.ai"
export ANTHROPIC_API_KEY="YOUR_FREE_OPENROUTER_KEY"
export ANTHROPIC_MODEL="meta-llama/llama-3-8b-instruct:free"
claude
```

---

## 🔄 Bypass Rate Limits with OmniRoute (Key Rotation)

Free tiers (like Google AI Studio or Groq) have strict requests-per-minute (RPM) limits. To prevent your Claude Code or Codex CLI from freezing during a long coding session, you can use **OmniRoute** as a local AI gateway. It automatically rotates multiple free keys using smart algorithms like *Headroom* (choosing the key with the most limits left) and compresses tokens to save budget.

### 🔌 Step 1: Install OmniRoute Local Server
Open your Windows CMD (or terminal) and install OmniRoute globally via NPM:

```cmd
npm install -g omniroute
```

### ⚙️ Step 2: Launch and Connect Keys
Start the omni-gateway by running:

```cmd
omniroute
```
*This will spin up a local server and display a temporary access token. Open `http://localhost:20128` in your browser, enter the token, and go to the **Providers** tab to connect your free Google AI Studio keys or OpenRouter accounts.*

### 💻 Step 3: Route Your CLI Agents to the Omni-Pool

Open a new CMD window, navigate to your project directory, and point your favorite AI developer tools to OmniRoute's local endpoint:

#### For Claude Code CLI:
```cmd
set ANTHROPIC_BASE_URL=http://localhost:20128/v1
set ANTHROPIC_API_KEY=any_dummy_string
set ANTHROPIC_MODEL=gemini-2.5-pro
claude
```

#### For OpenAI Codex CLI:
```cmd
set OPENAI_BASE_URL=http://localhost:20128/v1
set OPENAI_API_KEY=any_dummy_string
set OPENAI_MODEL=gemini-2.5-pro
codex --approval-mode full-auto
```

---
*Contributions, suggestions, and stars are highly appreciated! Let's build the ultimate resource for free AI coding tools together.*
