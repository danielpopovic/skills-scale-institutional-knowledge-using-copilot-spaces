# OctoAcme — Design and User Research Guide

## Purpose
This document establishes UX/UI design processes and user research practices for OctoAcme projects. It defines how the design function integrates with product and engineering at each project phase.

---

## UX/UI Designer Role

### Responsibilities
- Design user interfaces and interaction flows for new features
- Conduct and synthesize usability studies and user research
- Maintain and extend the shared design system
- Produce design specifications and annotated handoff files for engineers
- Conduct design reviews and iterate based on feedback
- Advocate for accessibility and inclusive design across the team

### When Designers are involved
- **Initiation:** Contribute to user research planning and early problem framing
- **Planning:** Create wireframes, prototypes, and detailed design specs before development begins
- **Execution:** Collaborate with Developers during implementation; review builds for design fidelity
- **Release:** Validate that the shipped experience matches approved designs
- **Retrospective:** Debrief on user feedback and identify UX improvements for future iterations

---

## Design Workflow

### 1. Discovery and Research
- Align with Product Manager on user needs, business goals, and constraints
- Review existing user research, analytics data, and support feedback
- Define research questions and conduct usability studies or interviews as needed
- Synthesize findings into insights that inform the design approach

### 2. Ideation and Wireframing
- Produce low-fidelity wireframes or flows to explore solution approaches
- Share early concepts with Product Manager and Developers for feasibility feedback
- Iterate on wireframes based on feedback before moving to high-fidelity design

### 3. High-Fidelity Design
- Apply the OctoAcme design system (components, typography, color, spacing)
- Ensure designs meet accessibility standards (WCAG 2.1 AA minimum)
- Annotate designs with interaction specs, edge cases, and error states
- Produce a complete design spec covering all screen states

### 4. Design Review
- Share designs with the team for review (Product Manager, Developers, QA)
- Incorporate feedback and resolve open questions before handoff
- Document any trade-offs or deferred items for the design backlog

### 5. Handoff to Engineering
- Deliver final design files with specs via the shared design tool (e.g., Figma)
- Conduct a handoff walkthrough with the implementing Developers
- Remain available for design questions during implementation
- Use the design handoff template (see [Cross-Functional Interactions](octoacme-cross-functional-interactions.md))

### 6. Implementation Review
- Review implemented feature in staging for design fidelity
- Log any discrepancies as defects or design debt items
- Sign off on visual/interaction correctness before QA sign-off

---

## User Research Integration

### When to conduct research
- **Before planning** a major new feature (generative research)
- **During design** to validate concepts with usability testing (evaluative research)
- **After release** to measure usability improvements and identify new issues

### Research methods
| Method | When to use |
|---|---|
| User interviews | Early discovery; understanding context and needs |
| Usability testing | Validating wireframes or prototypes |
| Surveys | Gathering quantitative feedback at scale |
| Analytics review | Understanding current behavior and drop-off points |
| Card sorting | Validating information architecture |
| A/B testing | Comparing design variants with live users |

### Sharing research findings
- Summarize findings in a research brief and share with Product Manager and team
- Highlight actionable insights and recommended design changes
- Archive research artifacts for future reference

---

## Design System Maintenance

- The design system is the shared library of reusable components, patterns, and guidelines
- UX/UI Designer owns the design system in collaboration with Developers who maintain the code implementation
- New components should be proposed, reviewed, and documented before being added
- Existing components should be updated when design standards evolve

---

## Design Review Checklist
- [ ] Design aligns with approved acceptance criteria and user needs
- [ ] All screen states covered (empty, loading, error, success, edge cases)
- [ ] Accessibility requirements met (contrast, touch targets, labels)
- [ ] Design system components used consistently
- [ ] Design reviewed and approved by Product Manager
- [ ] Handoff assets and specs delivered to Developers
- [ ] Handoff walkthrough completed

---

## Related Documents
- [OctoAcme Roles and Personas](octoacme-roles-and-personas.md)
- [OctoAcme Cross-Functional Interactions](octoacme-cross-functional-interactions.md)
- [OctoAcme Project Planning](octoacme-project-planning.md)
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md)
