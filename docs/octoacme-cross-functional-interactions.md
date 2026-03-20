# OctoAcme — Cross-Functional Interactions

## Purpose
This document clarifies how all OctoAcme roles collaborate across each project phase, defines handoff points and approval requirements, and provides communication templates for role-to-role interactions.

---

## Collaboration by Project Phase

### 1. Initiation
| Activity | Primary Owner | Collaborators |
|---|---|---|
| Define problem statement & goals | Product Manager | Project Manager, Developers |
| Identify success metrics | Product Manager | Data Analysts |
| Scope UX research needs | UX/UI Designer | Product Manager |
| Assess infrastructure requirements | DevOps/Platform Engineer | Developers |
| Define QA strategy | QA/Test Engineer | Product Manager, Developers |

**Key outputs:** Project one-pager, initial metrics plan, UX research plan, infrastructure assessment

---

### 2. Planning
| Activity | Primary Owner | Collaborators |
|---|---|---|
| Roadmap and backlog prioritization | Product Manager | All roles |
| Sprint/milestone planning | Project Manager | Developers, QA, Designer |
| Design wireframes and specs | UX/UI Designer | Product Manager, Developers |
| Test plan creation | QA/Test Engineer | Developers, Product Manager |
| CI/CD and environment setup | DevOps/Platform Engineer | Developers |
| Analytics instrumentation plan | Data Analyst | Developers, Product Manager |

**Key outputs:** Prioritized backlog, design specs, test plan, environment runbook, instrumentation plan

---

### 3. Execution
| Activity | Primary Owner | Collaborators |
|---|---|---|
| Feature implementation | Developers | UX/UI Designer, QA |
| Design review and handoff | UX/UI Designer | Developers, Product Manager |
| Automated test development | QA/Test Engineer | Developers |
| CI/CD pipeline maintenance | DevOps/Platform Engineer | Developers, QA |
| Feature flagging and rollouts | DevOps/Platform Engineer | Developers, Product Manager |
| Metrics tracking and dashboards | Data Analyst | Developers, Project Manager |

**Handoff points:**
- Designer → Developer: Design spec approved, assets delivered, design review completed
- Developer → QA: Feature branch ready, unit tests passing, PR approved and merged

---

### 4. Release
| Activity | Primary Owner | Collaborators |
|---|---|---|
| QA sign-off | QA/Test Engineer | Developers, Product Manager |
| Release notes | Product Manager | Project Manager, Developers |
| Deployment execution | DevOps/Platform Engineer | Developers |
| Post-deploy verification | QA/Test Engineer | DevOps/Platform Engineer |
| Stakeholder announcement | Project Manager | Product Manager |
| Release metrics baseline | Data Analyst | Product Manager |

**Approval requirements before production deployment:**
1. QA/Test Engineer confirms all acceptance criteria pass
2. DevOps/Platform Engineer confirms deployment pipeline is healthy
3. Product Manager approves release notes
4. Project Manager confirms rollback plan is documented

---

### 5. Retrospective
| Activity | Primary Owner | Collaborators |
|---|---|---|
| Retrospective facilitation | Project Manager | All roles |
| Metrics review and insights | Data Analyst | Product Manager |
| QA process improvement review | QA/Test Engineer | Developers |
| UX research debrief | UX/UI Designer | Product Manager |
| Infrastructure improvement items | DevOps/Platform Engineer | Developers |

**Key outputs:** Action items by role, updated process documentation, improvement backlog items

---

## Decision-Making Patterns

### When roles disagree on scope or requirements
1. Product Manager has final authority on scope and prioritization
2. Escalate unresolved conflicts to Project Manager for facilitation
3. Document decisions and rationale in the project decision log

### When QA blocks a release
1. QA/Test Engineer documents the blocking defect with severity and steps to reproduce
2. Product Manager and Project Manager assess impact and decide: fix, defer, or accept risk
3. Decision is logged and communicated to stakeholders

### When infrastructure blocks development
1. DevOps/Platform Engineer documents the blocker and estimated resolution time
2. Project Manager escalates if resolution time impacts milestone
3. Team identifies a workaround where possible

### When design and engineering disagree on feasibility
1. UX/UI Designer and Developer discuss constraints directly
2. If unresolved, Product Manager facilitates a trade-off discussion
3. Agreed solution is documented in the design spec

---

## Communication Templates

### Design Handoff to Engineering
> **Design handoff: [Feature Name]**
> - Figma link: [URL]
> - Design spec summary: [brief description]
> - Open questions: [list any unresolved items]
> - Acceptance criteria checklist: [list visual/interaction checks]
> - Reviewer: [Developer name]

### QA Sign-Off for Release
> **QA Sign-Off: [Release Name / Version]**
> - Test plan executed: ✅ / ❌
> - Automated tests passing: ✅ / ❌
> - Manual acceptance criteria verified: ✅ / ❌
> - Open defects: [list with severity]
> - Recommendation: **APPROVED** / **BLOCKED** — [reason]
> - Signed off by: [QA Engineer name]

### DevOps Deployment Readiness
> **Deployment Readiness: [Release Name / Version]**
> - CI pipeline passing: ✅ / ❌
> - Staging deployment verified: ✅ / ❌
> - Rollback plan documented: ✅ / ❌
> - Deployment window confirmed: [date/time]
> - On-call contact: [name]

---

## Related Documents
- [OctoAcme Roles and Personas](octoacme-roles-and-personas.md)
- [OctoAcme Quality Assurance Guide](octoacme-quality-assurance-guide.md)
- [OctoAcme Design and User Research Guide](octoacme-design-and-user-research.md)
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md)
- [OctoAcme Release & Deployment Guide](octoacme-release-and-deployment.md)
