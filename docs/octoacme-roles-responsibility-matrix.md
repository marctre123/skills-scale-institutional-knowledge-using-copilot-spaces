# OctoAcme — Roles & Responsibility Matrix

## Purpose
Map every role to each project lifecycle phase, clarifying who is **Responsible (R)**, **Accountable (A)**, **Consulted (C)**, or **Informed (I)** for key activities. Use this matrix to resolve ownership questions and reduce hand-off gaps.

> **Key:** R = Responsible (does the work) · A = Accountable (final decision/sign-off) · C = Consulted (input required) · I = Informed (kept in the loop) · — = Not involved

For full role descriptions see [Roles & Personas](./octoacme-roles-and-personas.md).

---

## Lifecycle Phase Matrix

| Activity | Project Manager | Product Manager | Developer | UX/UI Designer | QA Engineer | Release Manager | Customer Support | Tech Writer |
|---|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | | |
| Problem statement & goals | C | A | C | C | — | — | C | — |
| Stakeholder identification | A | C | — | — | — | — | C | — |
| Project charter / one-pager | A | R | — | — | — | — | — | C |
| **Planning** | | | | | | | | |
| Backlog definition & acceptance criteria | C | A | C | C | C | — | C | — |
| User flows & design specs | C | C | C | A | C | — | — | C |
| Test plan ownership | — | C | C | — | A | — | — | — |
| Release calendar & deployment schedule | A | C | C | — | C | R | — | — |
| Risk register creation | A | C | C | — | — | C | — | — |
| **Execution** | | | | | | | | |
| Feature implementation | — | C | R | C | — | — | — | — |
| Design review & fidelity check | — | — | C | A | C | — | — | — |
| QA column triage & bug reporting | — | C | R | — | A | — | — | — |
| Documentation updates (process docs) | C | — | — | — | — | — | — | A |
| Status reporting | A | C | I | I | I | I | I | — |
| **Release** | | | | | | | | |
| Release readiness sign-off | C | A | C | — | R | A | I | — |
| Go / no-go decision | C | A | C | — | C | R | I | — |
| Deployment execution | — | — | C | — | — | A | — | — |
| Release notes authoring | C | C | C | — | — | R | C | A |
| Stakeholder / user communication | A | C | — | — | — | C | R | C |
| Rollback & incident escalation | A | C | R | — | C | A | C | — |
| **Retrospective** | | | | | | | | |
| Retrospective facilitation | A | C | C | C | C | C | C | C |
| Action item ownership | A | C | C | C | C | C | C | C |
| Documentation of lessons learned | C | — | — | — | — | — | — | A |

---

## Key Ownership Signals

### Backlog Definition and Acceptance Criteria
- **Accountable**: Product Manager
- **Responsible**: Product Manager authors; Developers, Designers, and QA contribute
- **Acceptance criteria must be defined before a ticket moves to "Ready"**

### Test Plan Ownership
- **Accountable**: QA Engineer
- **Responsible**: QA Engineer authors; Developers provide technical context
- **Test plans must be reviewed before sprint execution begins**

### Release Readiness and Sign-Off
- **Accountable**: Release Manager (deployment gate) and Product Manager (scope/feature gate)
- **Responsible**: QA Engineer provides test sign-off; Developers confirm CI is green
- **No deployment proceeds without explicit go/no-go from Release Manager**

### Incident Communication and Escalation
- **Accountable**: Release Manager (technical escalation) and Project Manager (stakeholder escalation)
- **Responsible**: Developer triages root cause; Customer Support handles user-facing communication
- See [Release & Deployment Guide](./octoacme-release-and-deployment.md) for the rollback playbook

### Documentation Updates
- **Accountable**: Technical Writer / Documentation Lead
- **Responsible**: Technical Writer updates; all roles are consulted when their area changes
- **PRs that change documented workflows should tag the Technical Writer for review**

---

## DRI (Directly Responsible Individual) Summary

| Deliverable | DRI |
|---|---|
| Product roadmap and backlog | Product Manager |
| Project plan, timeline, and risk register | Project Manager |
| Design specs and prototypes | UX/UI Designer |
| Test strategy and quality gate | QA Engineer |
| Deployment schedule and go/no-go | Release Manager |
| User communication and support escalations | Customer Support |
| Process and product documentation | Technical Writer |
| Feature implementation | Developer (assigned to ticket) |
