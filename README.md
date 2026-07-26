# Nishant Tyagi

**Junior AI / GenAI Engineer | LLM Evaluation, RAG & Python Backends**

I build reliable LLM applications, agent evaluation systems, RAG pipelines, and Python backends. I focus on deterministic testing, safety guardrails, and production reliability—so agent behavior can be measured, gated in CI, and improved without silent regressions.

## Featured Projects

### [AgentEval](https://github.com/nishanttyagi28/agenteval)

**CI for AI agents that turns production failures into minimized regression tests.**

Local-first evaluation harness for multi-step LLM agents:

- YAML golden suites with correctness, hallucination, tool-call accuracy, latency, and cost
- **Production Failure Memory** (v0.3.0): redaction before persistence, deterministic clustering, sync/async replay, automatic failure minimization, human-approved golden export, recurrence and resurfacing detection
- GitHub Actions regression gates and local SQLite storage
- Zero-network demo path (no API key required for the flagship Failure Memory demo)

**Release verification (v0.3.0):** 1115 passed, 1 skipped

| | |
|---|---|
| Repository | https://github.com/nishanttyagi28/agenteval |
| PyPI | https://pypi.org/project/nishanttyagi-agenteval/ (`nishanttyagi-agenteval` · CLI/import: `agenteval`) |
| Release | https://github.com/nishanttyagi28/agenteval/releases/tag/v0.3.0 |
| Static demo | https://nishanttyagi28.github.io/agenteval/ |
| Dashboard | https://agenteval-6honbe24hradazngswxkrq.streamlit.app/ |

### [Agentic Data Analyst](https://github.com/nishanttyagi28/agentic-data-analyst)

Multi-agent Streamlit app for natural-language analysis of uploaded CSVs: quality gates, text-to-SQL (Groq Llama 3.3 70B), EDA/AutoML, forecasting, and ChromaDB RAG follow-ups.

[Live demo](https://agentic-data-analyst-uqjwnx2jwzd2pe9vosnffw.streamlit.app/)

### [Scheme Saathi](https://github.com/nishanttyagi28/scheme-saathi)

Government scheme eligibility navigator for Indian citizens. Rules-engine-first (deterministic), with optional local RAG (ChromaDB) and LangGraph + Groq for conversational guidance. FastAPI + Streamlit.

### [Contract Shield](https://github.com/nishanttyagi28/contract-shield)

Freelancer contract risk reviewer: deterministic rules plus Groq for plain-language explanations. FastAPI backend and Streamlit UI for PDF/DOCX/TXT uploads and risk reports.

## Technical focus

Python · FastAPI · Streamlit · LangGraph · Groq · Llama 3.3 70B · ChromaDB · SQL · SQLite · GitHub Actions · pytest · Docker

## Current flagship release

**AgentEval v0.3.0** — Failure Memory, deterministic replay/minimization, and CI regression protection for production agent failures.

Install: `pip install nishanttyagi-agenteval==0.3.0`

## Contact

- GitHub: [nishanttyagi28](https://github.com/nishanttyagi28)

---

*Built with a focus on verifiable, working systems. Open to Junior AI Engineer, GenAI Engineer, LLM Developer, and Python Backend opportunities.*
