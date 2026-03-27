# Decision Log Template

Maintain a running log of significant project decisions to support transparency and reduce repeated context-switching. Add a new row for each decision as it is made.

See [Project Planning](../octoacme-project-planning.md) and [Execution & Tracking](../octoacme-execution-and-tracking.md) for guidance on when to log decisions.

---

## [Project Name] — Decision Log

| ID | Date | Decision | Rationale | Alternatives Considered | Owner (DRI) | Status | Review Date |
|----|------|----------|-----------|------------------------|-------------|--------|-------------|
| D-001 | YYYY-MM-DD | Short description of what was decided | Why this option was chosen | What else was evaluated | [Name / Role] | Accepted / Superseded | YYYY-MM-DD |

---

## How to Use This Log

1. **Add a row** each time a significant, hard-to-reverse, or cross-team decision is made.
2. **Include rationale** so future team members understand the context without needing to track down meeting recordings or chat threads.
3. **Record alternatives** to capture trade-offs that were consciously evaluated.
4. **Assign a DRI** (Directly Responsible Individual) — the single person accountable for carrying out or championing the decision.
5. **Set a review date** for decisions that may need revisiting (e.g., tech choices, process changes).
6. **Update status** to "Superseded" if a later decision overrides an earlier one; add a reference to the new decision ID.

## Decision Categories (optional tags)
- `architecture` — technical design choices
- `product` — scope, prioritization, feature trade-offs
- `process` — how the team works
- `vendor` / `tooling` — third-party choices
- `security` — security posture or compliance decisions

---

*Template version: 1.0 — Store this file in the project repo (e.g., `docs/`) and link from the project README or meeting notes.*
