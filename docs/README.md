# OctoAcme Project Management Docs

**Abbreviations:** **PM** = Project Manager · **PdM** = Product Manager (Product Lead) · **DRI** = Directly Responsible Individual

## Overview

OctoAcme follows a lightweight, end-to-end project lifecycle: **Initiation → Planning → Execution → Release → Close/Retrospective**. Every initiative begins with a **Project Initiation** phase that validates the business need, confirms stakeholders, and defines measurable success criteria. The minimum deliverables are a **Project One-pager** (problem statement, goal, and success metrics), a stakeholder/communication plan, a high-level timeline with milestones, an initial risk list, and rough resourcing estimates. A clear decision gate ensures teams move forward only when success metrics, stakeholder alignment, and team availability are all confirmed.

## Key Workflows and Team Rhythm

Once approved, **Project Planning** turns the initiative into an actionable backlog and delivery plan: teams hold a kickoff, define a prioritized backlog with **acceptance criteria**, estimate work (T-shirt sizing or story points), document a **Definition of Done**, and surface dependencies and integration points. During **Execution & Tracking** the team works from a project board (e.g., GitHub Projects) with columns: **Backlog → Ready → In Progress → In Review → QA → Done**. The standard team rhythm includes **daily standups**, a **weekly delivery sync** for progress and risk review, and **demos/reviews** at the end of sprints or milestones. Risks and cross-team dependencies are tracked via a **Risk Register** (impact, likelihood, owner, mitigation, status) and escalated through regular syncs.

## Personas, Communication, and Quality Assurance

OctoAcme defines the following core and extended personas: the **PM (Project Manager)** coordinates delivery, timelines, risks, and communications; the **PdM (Product Manager)** defines outcomes, prioritizes the backlog, and measures success; **Developers** implement, test, and review changes; **QA/Testing** validates quality against acceptance criteria; **Tech Lead** provides technical direction; **DevOps/SRE** manages pipelines and reliability; **Scrum Master** facilitates agile ceremonies; **UX Designer** ensures usability; **Security Champion** embeds security in the development process; and **Stakeholder/Sponsor** provides strategic direction and escalation authority. Each backlog item, risk, and action item must have a single **DRI** (Directly Responsible Individual).

Communication is structured around a weekly PM + PdM sync, twice-weekly team standups, monthly stakeholder updates, and ad-hoc escalations. Quality is built into the development workflow: PRs are encouraged to be small (≤ 400 lines when possible), must link to the related issue and acceptance criteria, and must pass automated CI and security checks before review. At least one peer approval is required per team policy, and testing expectations include **unit tests** for new logic, **integration tests** where relevant, and **end-to-end smoke tests** for critical flows.

## Release, Retrospectives, and Continuous Improvement

Releases follow a standardized checklist: staging deploy and smoke tests, production deploy, post-deploy verification, and stakeholder announcements, with rollback and incident guidance in place. After milestones, sprints, or incidents, teams run structured **retrospectives** that produce owned, time-bound action items tracked back in the backlog for continuous improvement. Velocity, burndown, and outcome metrics are used to monitor progress and inform future planning cycles.

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, lifecycle, core roles, and key artifacts |
| [Project Initiation Guide](octoacme-project-initiation.md) | Decision gates, one-pager template, stakeholder plan |
| [Project Planning](octoacme-project-planning.md) | Backlog, milestones, estimation, Definition of Done |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Project board states, standups, DRI ownership, metrics |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, communication cadence |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, rollback guidance, announcements |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro format, action item tracking, improvement loop |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and goals for each persona |

## Templates

Ready-to-use templates for recurring project artifacts:

| Template | Description |
|---|---|
| [Project One-Pager](templates/project-one-pager-template.md) | Structured initiation document for validating and authorizing a project |
| [Weekly Status Update](templates/weekly-status-update-template.md) | Standardized weekly progress report for stakeholders |
| [Release Notes](templates/release-notes-template.md) | Structured release notes covering changes, migration steps, and announcements |
| [Decision Log](templates/decision-log-template.md) | Running log of significant decisions with rationale and DRI |
| [Meeting Notes](templates/meeting-notes-template.md) | Capture agenda, discussion, decisions, and action items for any meeting |

## Checklists

Checklists to enforce repeatable execution and quality gates:

| Checklist | Description |
|---|---|
| [Definition of Done](checklists/definition-of-done-checklist.md) | Minimum conditions for a backlog item to be marked Done |
| [Risk Register](checklists/risk-register-template.md) | Full risk tracking table with scoring guide and escalation triggers |

> Please keep this README updated as new process docs, templates, or checklists are added or revised.

