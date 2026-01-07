# OctoAcme Project Management Docs

This folder contains OctoAcme's program management process documents and a short introduction to how we run projects. The goal is to give teams clear, repeatable guidance for going from idea to production while keeping stakeholders aligned and product outcomes measurable.

OctoAcme follows a lifecycle of Initiation → Planning → Execution → Release → Close/Retrospective. Initiation captures the business need, stakeholders, and success metrics in a Project One‑pager. Planning breaks approved initiatives into a prioritized backlog with acceptance criteria, estimates, dependencies, and a release plan. Execution uses a visible project board and small, reviewable pull requests to move work through Ready → In Progress → In Review → QA → Done. Releases require passing CI, smoke tests, and a rollback plan; retrospectives capture learnings and convert them into tracked action items.

Roles are explicit: Product Managers own outcomes and prioritization; Project Managers coordinate schedules, risks, and cross-team communication; Developers build and test; QA validates acceptance; stakeholders provide input and approvals. Communication is structured — daily standups for blockers, weekly delivery syncs and PM–PdM alignment, demos at the end of sprints/milestones, and monthly stakeholder updates — with templates and escalation paths to keep information flowing.

Quality assurance is integrated into day-to-day work: unit and integration tests, end-to-end smoke tests, CI-based security scans, and manual QA where needed. PR rules enforce linked issues, acceptance criteria, passing CI, and required approvals. Release checklists, rollback playbooks, and post-incident retrospectives reduce production risk and support continuous improvement.

## Docs Index

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risks & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](octoacme-roles-and-personas.md)

## How to use these docs

- Keep the Project One-pager and release notes in the project repo and reference these process docs as the canonical guide.
- Add action items from retrospectives to the project backlog and track them in weekly PM syncs.
- If you want Copilot Spaces to use a process doc as context, add it to `.copilot/` as described in the Project Management Overview.
