# Nishant Tyagi

AI Engineer. I build and ship evaluation, runtime-trust, and multi-agent systems.

[Portfolio](https://nishant-tyagi-six.vercel.app) · [PyPI](https://pypi.org/project/nishanttyagi-agenteval/) · [AgentEval](https://github.com/nishanttyagi28/agenteval) · [KarmaSakshi](https://github.com/nishanttyagi28/karmasakshi-protocol)

**Shipped**

- **AgentEval** — published PyPI package (`nishanttyagi-agenteval`, v0.5.0). Deterministic test suite. CI regression gates. Failure Memory. Adapters for LangGraph, CrewAI, AutoGen, and the OpenAI Agents SDK.
- **KarmaSakshi Protocol** — runtime trust protocol: cryptographic effect sealing, TOCTOU revalidation, exactly-once execution, independent verification, Action Passports. Security invariants documented and mapped to tests.
- **Agentic Data Analyst** — live multi-agent analytics: text-to-SQL, AutoML, forecasting, statistical tests, RAG.
- Personal site in **TypeScript / Next.js 15** — [portfolio](https://nishant-tyagi-six.vercel.app), deployed on Vercel.

## Featured projects

### [AgentEval](https://github.com/nishanttyagi28/agenteval)

Evaluation infrastructure for AI agents. YAML goldens, baseline compare, and PR gates for correctness, tools, trajectories, flakiness, RAG, and cost. Failure Memory: redact → cluster → replay → minimize → human approve → CI.

```text
pip install nishanttyagi-agenteval
```

v0.5.0, alpha. Local-first. Nothing auto-enters blocking CI.

[Repo](https://github.com/nishanttyagi28/agenteval) · [PyPI](https://pypi.org/project/nishanttyagi-agenteval/) · [v0.5.0](https://github.com/nishanttyagi28/agenteval/releases/tag/v0.5.0) · [Dashboard](https://agenteval-6honbe24hradazngswxkrq.streamlit.app/)

### [KarmaSakshi Protocol](https://github.com/nishanttyagi28/karmasakshi-protocol)

Runtime protocol for consequential agent actions. Approval is bound to one sealed effect, not a tool name. Commit-time TOCTOU checks. Exactly-once reservation. Independent re-observation. Audit chain + Action Passport. The agent never holds a signing key.

v0.2.0 experimental, evaluation-ready — not a certified payment product. `mypy` strict mode in CI.

[Repo](https://github.com/nishanttyagi28/karmasakshi-protocol) · [PyPI](https://pypi.org/project/karmasakshi-protocol/)

### [Agentic Data Analyst](https://github.com/nishanttyagi28/agentic-data-analyst)

Multi-agent system behind one chat: quality gate, SELECT-only SQL, stats, forecasts, AutoML with leakage flags, HTML reports, ChromaDB session memory.

[Repo](https://github.com/nishanttyagi28/agentic-data-analyst) · [Live](https://agentic-data-analyst-uqjwnx2jwzd2pe9vosnffw.streamlit.app/)

## Engineering

- Gate agent behavior in CI. A green demo is not a regression test.
- Verify the approved effect at runtime. Allow/deny is not proof.
- Keep scores honest. Provider and evaluator failures are not agent failures.

## Current focus

AgentEval and KarmaSakshi as a pair: offline regression gates plus runtime verification for actions that hit money, mail, or data.

Python · pytest · GitHub Actions · LangGraph · FastAPI · TypeScript · Next.js

## Links

[Portfolio](https://nishant-tyagi-six.vercel.app) · [GitHub](https://github.com/nishanttyagi28) · [LinkedIn](https://www.linkedin.com/in/nishant-tyagi-7aa458356) · [X](https://x.com/tnishant838)
