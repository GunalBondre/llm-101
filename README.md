# 🤖 Frontend → Full-Stack AI Engineer

### The Complete LLM Engineering Course

> Built for developers with frontend experience who want to break into AI engineering at $100k+

---

## 📺 YouTube Series

Follow along: **[link coming soon]**

Each module has a companion YouTube video. Notebooks are designed to run alongside the video.

---

## 🗂️ Course Structure

```
llm-101/
│
├── module-00-foundations/           # How LLMs actually work
│   ├── 01_tokens_and_costs.ipynb
│   ├── 02_transformer_intuition.ipynb
│   ├── 03_llm_comparison.ipynb
│   └── 04_context_window_limits.ipynb
│
├── module-01-prompting/             # Prompt engineering (the money skill)
│   ├── 01_zero_shot_vs_few_shot.ipynb
│   ├── 02_chain_of_thought.ipynb
│   ├── 03_structured_output.ipynb
│   ├── 04_system_prompt_design.ipynb
│   └── 05_prompt_evaluation.ipynb
│
├── module-02-apis/                  # LLM APIs & integrations
│   ├── 01_openai_sdk_deep_dive.ipynb
│   ├── 02_multi_provider_abstraction.ipynb
│   ├── 03_streaming_ui_integration.ipynb
│   └── 04_cost_and_rate_limits.ipynb
│
├── module-03-rag/                   # Retrieval-Augmented Generation
│   ├── 01_embeddings_explained.ipynb
│   ├── 02_vector_databases.ipynb
│   ├── 03_basic_rag_pipeline.ipynb
│   ├── 04_chunking_strategies.ipynb
│   ├── 05_rag_evaluation.ipynb
│   └── 06_advanced_rag.ipynb
│
├── module-04-agents/                # AI Agents & tool use
│   ├── 01_function_calling_deep_dive.ipynb
│   ├── 02_react_agent_from_scratch.ipynb
│   ├── 03_tool_use_patterns.ipynb
│   ├── 04_memory_systems.ipynb
│   ├── 05_multi_agent_systems.ipynb
│   └── 06_agent_evaluation.ipynb
│
├── module-05-capstone/              # Full-stack AI app (end-to-end)
│   ├── 01_architecture_design.ipynb
│   ├── 02_backend_api_design.ipynb
│   ├── 03_frontend_ai_patterns.ipynb
│   ├── 04_database_schema.ipynb
│   ├── 05_testing_ai_apps.ipynb
│   └── 06_deployment_checklist.ipynb
│
└── module-06-production/            # Prod, evals & getting hired
    ├── 01_observability.ipynb
    ├── 02_evals_framework.ipynb
    ├── 03_prompt_versioning.ipynb
    └── 04_portfolio_strategy.ipynb
```

> 35 notebooks · 7 modules · ~17 weeks

---

## ⚡ Setup Guide

### 1. Clone the Starter Template

To follow along with all empty placeholder notebooks from scratch, clone the `starter-template` branch:

```bash
git clone -b starter-template https://github.com/GunalBondre/llm-101.git
cd llm-101
```

> 📌 **Starter Branch Link**: [github.com/GunalBondre/llm-101/tree/starter-template](https://github.com/GunalBondre/llm-101/tree/starter-template)

---

### 🍎 macOS Setup

#### Step 1 — Install Python 3.11+

**Option A: Homebrew (Recommended)**

If you don't have Homebrew installed, install it first:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then install Python:

```bash
brew install python@3.11
```

Add it to your PATH (add this to `~/.zshrc`):

```bash
echo 'export PATH="$(brew --prefix)/opt/python@3.11/libexec/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

Verify:

```bash
python3 --version   # Should show Python 3.11.x
```

**Option B: pyenv (Best for managing multiple Python versions)**

```bash
brew install pyenv
pyenv install 3.11
pyenv global 3.11
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
source ~/.zshrc
python --version   # Should show Python 3.11.x
```

#### Step 2 — Create a Virtual Environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Your terminal prompt should now show `(.venv)`.

#### Step 3 — Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

#### Step 4 — Set Up API Keys

```bash
cp .env.example .env
open .env   # Opens in TextEdit — add your API keys
```

#### Step 5 — Launch JupyterLab

```bash
jupyter lab
```

Then open `module-00-foundations/01_tokens_and_costs.ipynb` 🚀

**macOS Troubleshooting**

| Problem | Fix |
|---------|-----|
| `python3: command not found` | Run `brew install python@3.11` |
| `pip: command not found` | Run `python3 -m pip install --upgrade pip` |
| JupyterLab won't open in browser | Navigate manually to `http://localhost:8888` |
| SSL certificate errors | Run `brew install ca-certificates` |

---

### 🪟 Windows Setup

#### Step 1 — Install Python 3.11+

**Option A: winget (Recommended — built into Windows 10/11)**

Open **PowerShell as Administrator** (Win + X → Terminal Admin):

```powershell
winget install -e --id Python.Python.3.11
```

Close and reopen your terminal, then verify:

```powershell
python --version   # Should show Python 3.11.x
```

> ⚠️ **If `python` opens the Microsoft Store instead:** Go to **Settings → Apps → Advanced app settings → App execution aliases** and toggle **OFF** `python.exe` and `python3.exe`.

**Option B: Official Installer**

1. Download from [python.org/downloads](https://www.python.org/downloads/)
2. Run the installer — **✅ check "Add Python to PATH"** before clicking Install
3. Verify in a new terminal: `python --version`

#### Step 2 — Create a Virtual Environment

Open **PowerShell** or **Command Prompt** in the project folder:

```powershell
python -m venv .venv
.venv\Scripts\activate
```

Your prompt should now show `(.venv)`.

> ⚠️ **If you get a script execution error in PowerShell**, run this once:
> ```powershell
> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```

#### Step 3 — Install Dependencies

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

#### Step 4 — Set Up API Keys

```powershell
copy .env.example .env
notepad .env   # Add your API keys and save
```

#### Step 5 — Launch JupyterLab

```powershell
jupyter lab
```

Then open `module-00-foundations/01_tokens_and_costs.ipynb` 🚀

**Windows Troubleshooting**

| Problem | Fix |
|---------|-----|
| `python` opens Microsoft Store | Disable App Execution Aliases in Settings |
| `pip` not recognized | Run `python -m pip install --upgrade pip` |
| `.venv\Scripts\activate` fails | Run `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser` |
| JupyterLab won't open | Navigate manually to `http://localhost:8888` |
| `pip install` permission error | Run PowerShell as Administrator |

---

## 🔑 Required API Keys

| Service   | Where to get it                                        | Cost                      |
| --------- | ------------------------------------------------------ | ------------------------- |
| OpenAI    | [platform.openai.com](https://platform.openai.com)     | ~$5 credit free on signup |
| Anthropic | [console.anthropic.com](https://console.anthropic.com) | ~$5 credit free           |
| Others    | Added per module                                       | Free tiers available      |

---

## 🛠️ Tech Stack

- **Python 3.11+** — primary language
- **Jupyter Lab** — all notebooks run here
- **OpenAI SDK** — primary LLM provider
- **LangChain** — orchestration framework
- **Supabase / Chroma** — vector databases (Module 3+)

---

## 📊 Progress Tracker

- [x] Setup ✅
- [ ] Module 0 — Foundations
- [ ] Module 1 — Prompt Engineering
- [ ] Module 2 — APIs & Integrations
- [ ] Module 3 — RAG
- [ ] Module 4 — Agents
- [ ] Module 5 — Capstone Project
- [ ] Module 6 — Production & Hiring

---

_Made with ❤️ for the frontend dev who wants to build the future_
