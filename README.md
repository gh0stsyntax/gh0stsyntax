# Hi, I'm Nico 👋

M.Sc. Data Engineering & Consulting (2026), formerly RPA developer (UiPath, SAP process automation).
I work with AI coding agents every day and I care most about the part people skip: **proving that what the agent produced actually works** – and noticing when it doesn't.

## Featured

**[airlock](https://github.com/gh0stsyntax/airlock)** – a small, tested gate between agents and their tools: allowlist per agent, risk classes, approval with dry-run as the default, call budgets, hash-chained audit log. 16 tests, and the tests themselves are checked by breaking the code on purpose (8/8 mutations caught).

**[flowsmith](https://github.com/gh0stsyntax/flowsmith)** – plain language → UiPath workflow with a local LLM. The project's own quality score said 84–99/100, the real UiPath build said 0/5 – so the compiler was fixed until every output builds (5/5), each fix pinned by a regression test.

## How I work with agents

- Specification first, then tests the agent can run, then review of what it claims
- Least privilege and approval gates for anything that leaves the machine
- Evidence over verdicts: "N passed", not "looks good"; real toolchain instead of a heuristic score
- Parallel agents on isolated worktrees, merged by me

## Stack

Python · TypeScript · FastAPI · SQLite/PostgreSQL basics · Docker basics · Linux · UiPath · Ollama / local LLMs · Claude Code, OpenCode
