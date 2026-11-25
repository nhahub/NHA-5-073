# DistriMind

Agentic AI System for FMCG Distribution & Retail (DEPI capstone, AI & Data Science track).

**Team:** Ahmed Shawly, Moataz Adel Mohamed, Ahmed Elsaid Taha, Karim Mohamed Saeed Tohamy

**Status:** project structure only. No implementation yet.

## Structure

| Path | What it is | Owner |
|---|---|---|
| `app/main.py`, `app/api/` | FastAPI backend and endpoints | Karim |
| `app/schemas.py` | Shared contracts for all tools | All (change by agreement) |
| `app/orchestrator/` | LangGraph orchestrator | Unassigned |
| `app/agents/forecasting/` | Demand forecasting | Ahmed Shawly |
| `app/agents/inventory/` | Inventory and replenishment | Moataz |
| `app/agents/routing/` | Route and delivery planning | Moataz |
| `app/agents/pricing/` | Pricing and promotion | Ahmed Elsaid |
| `app/agents/retailer/` | Retailer assistant (RAG, lookup, memory) | Ahmed Elsaid |
| `app/core/` | Settings, logging, database, security, tracing | Karim |
| `app/rules/` | Approval and margin rules | Shared |
| `dashboard/` | Streamlit dashboard | Karim |
| `db/` | PostgreSQL schema | Ahmed Shawly |
| `data/` | Synthetic data scripts and knowledge documents | Ahmed Shawly, Ahmed Elsaid |
| `models/` | Trained model artifacts | Ahmed Shawly |
| `tests/` | Unit, contract, tool, workflow, safety, end-to-end tests | Everyone |
| `docs/` | Architecture, Team Brief, decision log | Everyone |

## Working rules

1. One repo. Work on your own branch and merge through pull requests.
2. Work inside your own folder. Change `app/schemas.py` only by team agreement.
3. Every agent merges a working stub first, then the real logic.
4. No invented data. Label synthetic data as synthetic.
5. Report status honestly: implemented, tested, evaluated, deployed only when true.
6. Record team decisions in `docs/decision-log.md`.
