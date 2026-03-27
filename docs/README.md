# OctoAcme Project Management Docs

## Overview

OctoAcme follows a lightweight, end-to-end project lifecycle: **Initiation → Planning → Execution → Release → Close/Retrospective**. Every initiative begins with a **Project Initiation** phase that validates the business need, confirms stakeholders, and defines measurable success criteria. The minimum deliverables are a **Project One-pager** (problem statement, goal, and success metrics), a stakeholder/communication plan, a high-level timeline with milestones, an initial risk list, and rough resourcing estimates. A clear decision gate ensures teams move forward only when success metrics, stakeholder alignment, and team availability are all confirmed.

## Key Workflows and Team Rhythm

Once approved, **Project Planning** turns the initiative into an actionable backlog and delivery plan: teams hold a kickoff, define a prioritized backlog with **acceptance criteria**, estimate work (T-shirt sizing or story points), document a **Definition of Done**, and surface dependencies and integration points. During **Execution & Tracking** the team works from a project board (e.g., GitHub Projects) with columns: **Backlog → Ready → In Progress → In Review → QA → Done**. The standard team rhythm includes **daily standups**, a **weekly delivery sync** for progress and risk review, and **demos/reviews** at the end of sprints or milestones. Risks and cross-team dependencies are tracked via a **Risk Register** (impact, likelihood, owner, mitigation, status) and escalated through regular syncs.

## Personas, Communication, and Quality Assurance

OctoAcme defines four core personas: the **Project Manager (PM)** coordinates delivery, timelines, risks, and communications; the **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures success; **Developers** implement, test, and review changes; and **QA/Testing** validates quality against acceptance criteria. Communication is structured around a weekly PM + PdM sync, twice-weekly team standups, monthly stakeholder updates, and ad-hoc escalations. Quality is built into the development workflow: PRs are encouraged to be small (≤ 400 lines when possible), must link to the related issue and acceptance criteria, and must pass automated CI and security checks before review. At least one peer approval is required per team policy, and testing expectations include **unit tests** for new logic, **integration tests** where relevant, and **end-to-end smoke tests** for critical flows.

## Release, Retrospectives, and Continuous Improvement

Releases follow a standardized checklist: staging deploy and smoke tests, production deploy, post-deploy verification, and stakeholder announcements, with rollback and incident guidance in place. After milestones, sprints, or incidents, teams run structured **retrospectives** that produce owned, time-bound action items tracked back in the backlog for continuous improvement. Velocity, burndown, and outcome metrics are used to monitor progress and inform future planning cycles.

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, lifecycle, core roles, and key artifacts |
| [Project Initiation Guide](octoacme-project-initiation.md) | Decision gates, one-pager template, stakeholder plan |
| [Project Planning](octoacme-project-planning.md) | Backlog, milestones, estimation, Definition of Done |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Project board states, standups, metrics |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, communication cadence |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, rollback guidance, announcements |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro format, action item tracking, improvement loop |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and goals for each persona |

> Please keep this README updated as new process docs are added or revised.
