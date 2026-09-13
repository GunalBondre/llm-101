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

## ⚡ Quick Setup (5 minutes)

### 1. Clone the repo

```bash
git clone <repo-url>
cd llm-101
```

### 2. Create a virtual environment

```bash
python -m venv .venv
or
python3 -m venv .venv
source .venv/bin/activate        # Mac/Linux
# .venv\Scripts\activate         # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your API keys

```bash
cp .env.example .env
# Open .env and add your OpenAI key
```

### 5. Launch Jupyter

```bash
jupyter lab
```

Then open `module-00-foundations/01_tokens_and_costs.ipynb` 🚀

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
