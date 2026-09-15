# OctoAcme Project Management Documentation

This README is the central index and entry point for OctoAcme project management process documentation. Use it to navigate the full lifecycle guidance, role expectations, delivery workflows, communication practices, and release/retrospective standards.

## Overview

OctoAcme uses a lightweight, iterative project management approach centered on clear ownership, measurable outcomes, and small, testable delivery increments. Teams work from a shared project board, use structured planning and risk practices, and apply quality gates through CI, reviews, and release checklists.

## Table of Contents

- [OctoAcme Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## Project Management Processes — Summary

OctoAcme runs projects with a clear, iterative management cadence designed to keep work small, visible, and measurable. Work is organized on a project board with Backlog → Ready → In Progress → In Review → QA → Done columns and guided by a Pull Request workflow that favors small changes (target <= 400 lines), links PRs to issues with acceptance criteria, and requires CI (tests, lint, security scans) and at least one approval before merge. Projects begin with a lightweight initiation step — a Project One-pager that defines the problem, SMART objectives, and success metrics — and move to planning only after stakeholders agree and team availability is confirmed.

Roles and responsibilities are explicit: Product Managers (PdM) own outcomes and prioritization, Project Managers (PM) coordinate delivery, schedules, risks and communications, Developers implement and test features, and QA/Testing validate acceptance criteria. These personas are used to allocate accountability across artifacts (one-pager, backlog, Definition of Done, risk register, release notes) and to shape who runs kickoffs, who owns acceptance criteria, and who tracks follow-up actions from retrospectives.

Communication is structured and frequent: daily standups for progress and blockers, weekly delivery syncs to surface progress and risks, PM–PdM weekly alignment, and regular stakeholder updates (weekly or per milestone). Templates and escalation paths are provided — weekly status templates for concise updates and a three-level blocker escalation (team → PM → Product Lead → Sponsor) — and incident communication follows an incident playbook with triage summaries and post-incident retrospectives. The docs encourage a single source of truth (project README or release doc) and use project boards and risk registers to make dependencies visible.

Quality and release practices emphasize automated and manual verification at multiple layers. Development work should include unit tests and integration tests, with end-to-end smoke tests for critical flows; CI enforces passing tests, linting, and security scanning before reviews. Releases follow checklists (pre-release verification, staging smoke tests, rollback/mitigation plan) and have clear rollback/playbook steps for incidents. Continuous improvement is embedded via regular retrospectives that produce prioritized action items tracked back into the backlog so process changes are measured and iterated on over time.

## Quick Start / Quick Reference Scenarios

- **I am starting a new project** → Begin with [Project Initiation Guide](./octoacme-project-initiation.md)
- **I need to plan scope, milestones, and dependencies** → Use [Project Planning](./octoacme-project-planning.md)
- **I am managing day-to-day delivery and PR flow** → Follow [Execution & Tracking](./octoacme-execution-and-tracking.md)
- **I need to track or escalate a risk** → See [Risk Management & Communication](./octoacme-risks-and-communication.md)
- **I am preparing for deployment** → Use [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- **I am running a retro or tracking improvements** → See [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- **I need role expectations and ownership boundaries** → Review [Roles & Personas](./octoacme-roles-and-personas.md)

## Using these docs with Copilot Spaces

- Add this `docs/README.md` and the linked process docs as context in your Copilot Space.
- Prompt Copilot with your current phase (initiation, planning, execution, release, or retrospective) and ask it to apply the matching checklist/template.
- Reference role context (PdM, PM, Developer, QA) in prompts to get persona-specific outputs.
- Keep one source of truth (project README or release doc) updated so Copilot responses stay aligned with current project status.

## Acceptance Criteria

- [x] `docs/README.md` created as the central index for OctoAcme process docs
- [x] Includes overview, full docs table of contents, and quick-reference scenarios
- [x] Includes the required 3–4 paragraph process summary
- [x] Includes guidance for using these docs with Copilot Spaces
- [x] Uses relative links to all specified documents in `docs/`
