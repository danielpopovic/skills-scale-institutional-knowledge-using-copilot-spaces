# OctoAcme — Quality Assurance Guide

## Purpose
This document formalizes QA practices referenced in OctoAcme execution and release processes. It defines the QA role, testing workflows, acceptance criteria alignment, and the Definition of Done for all work item types.

---

## QA/Test Engineer Role

### Responsibilities
- Create and maintain test plans for all features and releases
- Build, maintain, and extend automated test suites (unit, integration, end-to-end)
- Execute manual testing for acceptance criteria validation
- Document, triage, and track defects to resolution
- Coordinate QA sign-off for releases
- Continuously improve testing practices and tooling

### When QA is involved
- **Planning phase:** Review acceptance criteria with Product Managers; contribute to the Definition of Done
- **Execution phase:** Write automated tests alongside feature development; perform exploratory testing
- **Release phase:** Execute final test plan, provide QA sign-off, support post-deploy verification

---

## Test Planning

### Test Plan Contents
Each feature or milestone should have a test plan that includes:
- **Scope:** Features and flows covered
- **Out of scope:** What is explicitly not tested
- **Test types:** Unit, integration, end-to-end, performance, security, manual acceptance
- **Environments:** Which environments will be used
- **Entry criteria:** What must be true before testing begins (e.g., feature deployed to staging)
- **Exit criteria:** What must be true to consider testing complete
- **Defect triage process:** Severity definitions and escalation path

### Test Types
| Test Type | Owner | When |
|---|---|---|
| Unit tests | Developer (with QA review) | During development |
| Integration tests | Developer + QA | During development / CI |
| End-to-end tests | QA/Test Engineer | Pre-release / CI |
| Exploratory testing | QA/Test Engineer | During execution |
| Acceptance testing | QA/Test Engineer + Product Manager | Pre-release |
| Regression testing | QA/Test Engineer | Pre-release |
| Smoke tests | QA/Test Engineer + DevOps | Post-deploy |

---

## Test Execution Workflow

1. **Entry:** Feature is deployed to the staging/QA environment
2. **Automated tests:** CI pipeline runs unit, integration, and regression tests
3. **Manual acceptance testing:** QA/Test Engineer validates acceptance criteria manually
4. **Exploratory testing:** QA/Test Engineer tests edge cases and out-of-scope scenarios
5. **Defect logging:** All defects are logged with steps to reproduce, severity, and screenshots
6. **Defect triage:** Developer and QA review defects together; prioritize for fix or defer
7. **Retest:** Fixed defects are retested before sign-off
8. **Sign-off:** QA/Test Engineer provides written sign-off (see template in [Cross-Functional Interactions](octoacme-cross-functional-interactions.md))

---

## Acceptance Criteria Alignment

### Process
- Product Manager writes acceptance criteria in user story format
- QA/Test Engineer reviews and clarifies ambiguities before development begins
- Developer and QA agree on which criteria will be verified automatically vs. manually
- Acceptance criteria are linked to test cases in the test plan

### Acceptance Criteria Format
> **Given** [context or precondition]
> **When** [action is taken]
> **Then** [expected outcome]

---

## Definition of Done

### For a User Story / Feature
- [ ] All acceptance criteria verified (automated and/or manual)
- [ ] Automated tests written and passing in CI
- [ ] No open critical or high-severity defects
- [ ] Code reviewed and approved
- [ ] Documentation updated (if applicable)
- [ ] QA/Test Engineer has provided sign-off

### For a Bug Fix
- [ ] Root cause identified and documented
- [ ] Fix implemented and unit/regression test added
- [ ] No regressions introduced
- [ ] QA/Test Engineer has retested and confirmed resolved

### For a Release
- [ ] Full regression suite passing
- [ ] Acceptance criteria for all release items verified
- [ ] No unresolved critical or high defects
- [ ] QA sign-off documented (see [Cross-Functional Interactions](octoacme-cross-functional-interactions.md))
- [ ] Smoke test plan ready for post-deploy execution

---

## Defect Severity Definitions

| Severity | Definition | SLA |
|---|---|---|
| Critical | System is unusable; data loss or security issue | Must fix before release |
| High | Core functionality broken; no workaround | Must fix before release |
| Medium | Feature partially broken; workaround available | Fix in next sprint |
| Low | Minor issue; cosmetic or edge case | Fix as time allows |

---

## QA Feature Completion Checklist
- [ ] Test plan created and reviewed with Product Manager
- [ ] Automated tests written (unit, integration, or E2E as applicable)
- [ ] Manual acceptance testing completed
- [ ] All critical and high defects resolved
- [ ] Regression suite passing
- [ ] QA sign-off documented
- [ ] Smoke tests ready for post-deploy verification

---

## Related Documents
- [OctoAcme Roles and Personas](octoacme-roles-and-personas.md)
- [OctoAcme Cross-Functional Interactions](octoacme-cross-functional-interactions.md)
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md)
- [OctoAcme Release & Deployment Guide](octoacme-release-and-deployment.md)
