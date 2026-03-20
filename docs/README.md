# OctoAcme Project Management Docs

Welcome! This README provides a gateway to OctoAcme's structured, collaborative project management practices. It summarizes our approach and links out to detailed, living documents for each phase of the project lifecycle.

## Project Management Processes: Summary

OctoAcme operates a structured, phase-based project lifecycle that moves work from initiation through execution and into continuous improvement. The process begins with **Project Initiation**, where teams validate business needs, align stakeholders, and create a lightweight Project One-pager that defines the problem, goals, and success metrics. Once approved, projects move into **Planning**, where work is broken into shippable increments with clear acceptance criteria, dependencies are mapped, and a release timeline is established. During **Execution**, teams follow a pull-request-driven workflow with automated testing and quality gates, managed via GitHub Projects boards with columns spanning from Backlog to Done. Finally, after **Release and Deployment**, teams conduct retrospectives to capture learnings and convert them into actionable improvements, creating a continuous feedback loop that strengthens future iterations.

OctoAcme defines clear ownership across three primary roles: **Project Managers** coordinate schedules, risks, and stakeholder communications; **Product Managers** define what should be built and prioritize the backlog; and **Developers** implement features while contributing to design, testing, and risk identification. This structure is supported by a consistent communication cadence that includes daily standups (15 minutes, focused on blockers and progress), weekly delivery syncs between PM and Product Manager, twice-weekly team standups, and monthly stakeholder updates. Ad-hoc escalation paths exist to surface blockers, moving from team-level triage to PM escalation to Product Lead involvement to sponsor-level escalation when necessary.

Quality is embedded throughout OctoAcme's delivery model through unit tests, integration tests, end-to-end smoke tests, security scanning in CI, and manual QA for feature acceptance. The process mandates small pull requests (≤400 lines when possible) with automated testing and linting before review, plus at least one approval before merging. Risk management runs parallel to execution, with a formal Risk Register capturing ID, description, impact, likelihood, owner, and mitigation plans—reviewed and updated weekly. Dependencies across teams are marked on the project board and escalated during weekly syncs. This dual focus on preventive quality measures and proactive risk communication helps OctoAcme minimize unplanned work and maintain transparency with stakeholders throughout the project lifecycle.

## Process Docs Index
- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](octoacme-roles-and-personas.md)

## Getting Started

New team members should:
1. Start with the [Project Management Overview](octoacme-project-management-overview.md) for a quick introduction
2. Reference the appropriate process document based on the project phase you're in (Initiation → Planning → Execution → Release → Retrospective)
3. Check the [Roles & Personas](octoacme-roles-and-personas.md) document to understand your role and responsibilities

## Contributing

To propose updates or additions to these process documents, please use the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template.

This helps ensure process improvements are reviewed and aligned with the team before being integrated into the documentation.