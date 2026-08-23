# Nishant Tyagi

AI Engineer working on **agent reliability**: evaluation before merge, verification at runtime, and safety at the effect boundary.

I build infrastructure for systems that act — not chat demos. The work is public.

[Portfolio](https://nishant-tyagi-six.vercel.app) · [AgentEval](https://github.com/nishanttyagi28/agenteval) · [PyPI](https://pypi.org/project/nishanttyagi-agenteval/) · [KarmaSakshi](https://github.com/nishanttyagi28/karmasakshi-protocol)

---

An agent can return a confident answer, call the wrong tool, invent a fact, or refund twice after a timeout. Unit tests prove the code still runs. They do not prove the agent still behaves, or that the approved real-world effect is what actually happened.

That gap is an engineering problem. I treat it as one.

## Selected work

### [AgentEval](https://github.com/nishanttyagi28/agenteval) — evaluation infrastructure

Git-native CI for multi-step LLM agents. YAML golden suites, versioned baselines, and pull-request gates for correctness, hallucination, tool-call accuracy, trajectory, flakiness, latency, cost, and RAG. **Failure Memory** (v0.3.0) turns a redacted production failure into a minimized, human-approved regression case.

Adapters: LangGraph, CrewAI, AutoGen, OpenAI Agents SDK, custom.

```text
pip install nishanttyagi-agenteval==0.3.0
```

v0.3.0 verification: **1115 passed, 1 skipped**. Failure Memory suite: **59 passed**. Local-first. Capture off by default. Nothing enters blocking CI without a human.

[Repository](https://github.com/nishanttyagi28/agenteval) · [PyPI](https://pypi.org/project/nishanttyagi-agenteval/) · [Release](https://github.com/nishanttyagi28/agenteval/releases/tag/v0.3.0) · [Dashboard](https://agenteval-6honbe24hradazngswxkrq.streamlit.app/) · [Docs](https://nishanttyagi28.github.io/agenteval/)

### [KarmaSakshi Protocol](https://github.com/nishanttyagi28/karmasakshi-protocol) — runtime trust

IAM, OAuth, and policy gates answer whether an agent *may* call a tool. They do not prove that the exact effect a human approved is the exact effect that executed.

KarmaSakshi binds approval to one canonical **Effect Manifest**, seals it, revalidates preconditions at commit time (TOCTOU), executes with **exactly-once** reservation semantics, independently re-observes the system of record, and issues an **Action Passport**. The agent never holds a signing key.

Status: v0.2.0 experimental, evaluation-ready self-hosted software — not a certified payment product. **1049 tests**, **74 security invariants**, **90.5% coverage**, `mypy --strict` clean.

[Repository](https://github.com/nishanttyagi28/karmasakshi-protocol) · [PyPI](https://pypi.org/project/karmasakshi-protocol/)

### [Agentic Data Analyst](https://github.com/nishanttyagi28/agentic-data-analyst) — multi-agent analysis

One orchestrator. Seven specialists. One chat. Quality gating, SELECT-only text-to-SQL, statistical tests, forecasting, AutoML with leakage flags, HTML reports, and ChromaDB memory so follow-ups are grounded in the session.

[Repository](https://github.com/nishanttyagi28/agentic-data-analyst) · [Live demo](https://agentic-data-analyst-uqjwnx2jwzd2pe9vosnffw.streamlit.app/)

## Engineering

- **Evaluation is the product.** If you cannot fail a pull request when an agent regresses, you have anecdotes.
- **Allowed is not verified.** Permission to call a tool is not proof the approved effect happened, once.
- **Metric integrity.** Provider timeouts and evaluator failures are not agent failures. A useful harness exposes real misses instead of hiding them.
- **Fail closed.** Stale world, tampered manifests, revoked grants, unsafe SQL — these are errors, not warnings.
- **Open source as proof.** Tests, threat models, and limitations ship in the same voice as the code.

## Current focus

Closing the loop between offline evaluation and runtime verification: production incidents become golden cases; golden cases become CI gates; consequential actions remain independently observable.

Python, pytest, GitHub Actions, LangGraph, FastAPI, SQLite, Ed25519, RAG evaluation, protocol design.

## Elsewhere

[nishant-tyagi-six.vercel.app](https://nishant-tyagi-six.vercel.app) · [LinkedIn](https://www.linkedin.com/in/nishant-tyagi-7aa458356) · [X](https://x.com/tnishant838)
