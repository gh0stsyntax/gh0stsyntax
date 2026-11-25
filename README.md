# Hi, I'm Nico 👋

M.Sc. Data Engineering & Consulting (2026), formerly RPA developer (UiPath, SAP process automation).
I work with AI coding agents every day and I care most about the part people skip: **proving that what the agent produced actually works** – and noticing when it doesn't.

## Featured

**[airlock](https://github.com/gh0stsyntax/airlock)** – a small, tested gate between agents and their tools: allowlist per agent, risk classes, approval with dry-run as the default, call budgets, hash-chained audit log. 26 tests, including a three-role example (researcher / builder / reviewer), and the tests themselves are checked by breaking the code on purpose (8/8 mutations on the library, 7/7 on the example).

**[flowsmith](https://github.com/gh0stsyntax/flowsmith)** – plain language → UiPath workflow with a local LLM. The project's own quality score said 84–99/100, the real UiPath build said 0/5 – so I built a measurement loop around the real toolchain and fixed the compiler failure class by failure class, each fix pinned by a regression test. Honest current number: **9 of 16 fresh generations build** (tasks I had not tuned on; small sample). It is a working tool with known limits, not a finished product.

**[agent-control-plane](https://github.com/gh0stsyntax/agent-control-plane)** – a reference implementation of a governance layer for AI agents: a policy decision point (allow / escalate / block), versioned tool contracts, PII masking and prompt-injection checks, and a signed bridge for external agents (HMAC, time window, idempotency). Standard library only, 42 tests. The connected ERP/CRM/mail systems are simulated, and the README says so.

**[reception-desk](https://github.com/gh0stsyntax/reception-desk)** – the server side of a Vapi phone agent that books salon appointments: tested date/time and booking rules (the model never computes dates, a booking needs explicit confirmation and is re-checked), an importable n8n workflow generated from the same code, and a parity test between both. A reconstruction of a prototype whose original workflow was lost; not yet tested with a live call or a real calendar.

## How I work with agents

- Specification first, then tests the agent can run, then review of what it claims
- Least privilege and approval gates for anything that leaves the machine
- Evidence over verdicts: "N passed", not "looks good"; real toolchain instead of a heuristic score
- Parallel agents on isolated worktrees, merged by me

## Stack

Python · TypeScript · FastAPI · SQLite/PostgreSQL basics · Docker basics · Linux · UiPath · Ollama / local LLMs · Claude Code, OpenCode
