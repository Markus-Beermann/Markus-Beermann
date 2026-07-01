# Hi, I'm Markus Beermann

I build practical AI systems with a strong focus on orchestration, traceability,
review gates, and human control. My current work is centered on multi-agent
engineering workflows: not decorative demos, but systems that can survive real
state, real blockers, and real operator decisions.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Markus%20Beermann-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/markusbeermann)
[![GitHub](https://img.shields.io/badge/GitHub-Markus--Beermann-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Markus-Beermann)

---

## What I Build

- Multi-agent AI systems with explicit roles, state, review gates, and audit trails
- LLM-backed engineering workflows across planning, implementation, review, and release
- PostgreSQL-centered control planes for agent state, lifecycle, and governance
- Practical automation around GitHub, CI, dashboards, migrations, and operator handoffs
- Local tools and small applications where usefulness matters more than presentation

I care about the part where agentic systems stop being impressive screenshots and
start being operational software.

---

## Cortex-Agentic

`Cortex-Agentic` is my private multi-agent AI operating system. It coordinates
specialized agent personas through a PostgreSQL-backed orchestration layer with
strict lifecycle tracking, review gates, and human approval for sensitive work.

The system is built around one core idea:

> The model may execute work, but the system owns truth, state, policy, and auditability.

### Core Architecture

```text
Human operator
  -> DB-backed task queue
  -> role-specific agent startup contract
  -> bounded implementation / review / planning session
  -> audited lifecycle update
  -> review gate
  -> controlled release
  -> post-merge hygiene
```

### Technical Components

- TypeScript / Node.js orchestration core with PostgreSQL-backed lifecycle and
  audit state
- Role-scoped agent workflows with review-gated releases and explicit human
  approval
- Operational safety checks around migrations, startup readiness, and release
  workflows
- GitHub, CI, and dashboard integrations for controlled engineering workflows

### Provider Strategy

Cortex-Agentic treats model providers as execution surfaces, not as the authority
layer. OpenAI, Anthropic, and other providers can be used where they fit, but
state, routing, lifecycle, and auditability stay under the local Cortex control
plane.

---

## Technical Focus

```text
Languages:       TypeScript, Python, SQL, JavaScript
Backend:         Node.js, Express, Flask
Data:            PostgreSQL, PL/pgSQL, schema migrations, audit tables
AI / LLMs:       OpenAI APIs, Anthropic SDK, multi-provider routing concepts
Frontend:        React, Next.js, CSS, mobile-first dashboard work
Automation:      GitHub CLI/API, CI checks, Vercel workflows, launchd/cron design
Testing:         Vitest, integration tests, migration tests, DB contract tests
Governance:      Review gates, lifecycle state machines, operator approvals
```

I am strongest where software engineering, AI systems, operational discipline,
and uncomfortable edge cases meet.

---

## Selected Projects

### Cortex-Agentic

Private multi-agent orchestration system for governed AI-assisted engineering.
The current version focuses on role separation, DB-first state, review gates,
audited writes, and safe handoffs between agents and human operator decisions.

### [universal-converter](https://github.com/Markus-Beermann/universal-converter)

Local macOS media converter built with Python, Flask, and FFmpeg. The goal is a
small, practical utility that handles common media conversion work locally without
turning a simple workflow into a cloud dependency.

### [youth-crisis-signal-protocol](https://github.com/Markus-Beermann/youth-crisis-signal-protocol)

Public exploration around signal protocols and crisis-oriented digital workflows.

---

## How I Think About AI Engineering

- Autonomy without observability is not engineering.
- Agent roles need contracts, not just names.
- Review and escalation are product features, not bureaucracy.
- Provider APIs are tools; the control plane should stay yours.
- State belongs somewhere inspectable.
- If the workflow cannot survive a failed run, stale clone, bad migration, or
  missing approval, it is not ready for serious work.

---

## Current Direction

I am building toward agentic systems that can:

- coordinate work across specialized AI agents
- preserve operational memory without relying on provider-local memory
- expose why a task is blocked, reviewed, merged, or paused
- combine model capability with database-backed governance
- remain useful when the happy path breaks

That last point matters most. Real systems fail in boring ways, and the boring
ways are where good engineering shows.

---

## Connect

- LinkedIn: [linkedin.com/in/markusbeermann](https://www.linkedin.com/in/markusbeermann)
- GitHub: [github.com/Markus-Beermann](https://github.com/Markus-Beermann)

---

> Quality before autonomy.
