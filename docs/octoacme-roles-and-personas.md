# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX/UI Designer

### Role Summary
UX/UI Designers translate product requirements into user-centered designs. They own the end-to-end design process from wireframes to high-fidelity prototypes and ensure usability standards are met before development begins.

### Responsibilities
- Create wireframes, mockups, and interactive prototypes
- Conduct usability reviews and gather user feedback
- Define and maintain design systems and component libraries
- Collaborate with Product Managers on user flows and feature requirements
- Review implemented features for design fidelity

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce rework by aligning design and implementation early
- Establish reusable design patterns to accelerate delivery

### Typical Communication
- Design review sessions with Developers and Product Managers
- Figma/design tool links shared in issues and PRs
- Usability feedback summarized in design decision docs

### Interactions with Other Roles
- **Developers**: Provides assets and answers implementation questions; reviews PRs for design accuracy
- **Product Managers**: Aligns on user flows, feature scope, and acceptance criteria during planning
- **QA Engineers**: Collaborates on usability test cases and reviews visual regressions
- **Project Managers**: Reports design milestone status; flags scope changes that affect timelines

---

## Quality Assurance (QA) Engineer

### Role Summary
QA Engineers ensure software meets acceptance criteria and quality standards before release. They own the test strategy, execute manual and automated testing cycles, and act as the quality gate between development and production.

### Responsibilities
- Define and maintain test plans and test cases aligned with acceptance criteria
- Execute manual and automated tests across environments (staging, regression, smoke)
- Triage and document defects; coordinate with Developers for resolution
- Own the **QA** column on the project board — items move here when development is complete and require verification
- Sign off on release readiness from a quality perspective

### Goals
- Prevent defects from reaching production
- Accelerate testing through automation and clear test coverage
- Provide fast, accurate feedback loops to Developers

### Typical Communication
- Bug reports filed as GitHub Issues with reproduction steps and severity
- Test results summarized in release readiness checklist
- Participates in sprint planning to scope test effort and in retros to flag quality trends

### Interactions with Other Roles
- **Developers**: Triages and validates bug fixes; pairs on testability improvements
- **Product Managers**: Clarifies acceptance criteria and edge cases during planning
- **Release Manager**: Provides test sign-off before deployment proceeds
- **UX/UI Designers**: Validates visual and interaction behavior against design specs
- **Customer Support**: Receives user-reported issues and validates fixes

---

## Release Manager

### Role Summary
Release Managers plan, coordinate, and execute releases across environments. They own the release schedule, change control process, release notes, and rollback plans.

### Responsibilities
- Maintain the release calendar and deployment schedule
- Coordinate release readiness reviews with QA, Developers, and Product Managers
- Prepare and publish release notes
- Manage deployment pipelines and orchestrate go/no-go decisions
- Own the rollback and incident escalation plan during deployments

### Goals
- Deliver predictable, low-risk releases
- Ensure all stakeholders are informed before and after releases
- Minimize production incidents through rigorous pre-release validation

### Typical Communication
- Release readiness reports shared with PM, PdM, and QA before each deployment
- Go/no-go announcements to the delivery team and stakeholders
- Post-release summaries and incident notes as needed

### Interactions with Other Roles
- **Developers**: Confirms all PRs are merged and CI is green before deployment
- **QA Engineers**: Requires test sign-off as part of the go/no-go decision
- **Product Managers**: Aligns on release timing and feature flags / staged rollouts
- **Project Managers**: Coordinates schedule and communicates dependencies or delays
- **Customer Support**: Provides advance notice of releases and known issues

---

## Customer Support / Success

### Role Summary
Customer Support and Success roles are the direct interface between users and the product team. They capture real-world user pain points, escalate issues, and ensure customers are informed and unblocked.

### Responsibilities
- Act as the first line of response for user-reported issues and feedback
- Triage incoming issues — distinguish bugs from user errors and document reproduction steps
- Escalate confirmed bugs and feature gaps to Product Managers and Developers
- Communicate known issues and workarounds to affected users
- Validate fixes with users to confirm resolution

### Goals
- Resolve user issues quickly and empathetically
- Surface actionable product insights to reduce repeat issues
- Build user trust through proactive communication during incidents

### Typical Communication
- Issue escalations filed as GitHub Issues or via PM/PdM channels
- Weekly summary of top user pain points shared with Product Managers
- Release-day communication to users (changelogs, known issues, workarounds)

### Interactions with Other Roles
- **Product Managers**: Shares user feedback and pain points to influence backlog prioritization
- **Developers**: Coordinates on urgent bug triage and hotfix validation
- **QA Engineers**: Provides real-world reproduction steps; validates fixes before closing escalations
- **Release Manager**: Receives advance release notes to prepare user communications
- **Project Managers**: Escalates customer-impacting issues that require plan changes

---

## Technical Writer / Documentation Lead

### Role Summary
Technical Writers maintain process and product documentation, ensuring that guides, runbooks, and onboarding materials remain accurate and accessible. They facilitate knowledge transfer across all roles.

### Responsibilities
- Own and maintain documentation under `docs/` and any product-facing guides
- Partner with all roles to capture process changes and new features in documentation
- Update onboarding materials when processes or tooling change
- Review PRs that impact documented workflows and flag gaps
- Establish documentation standards and templates

### Goals
- Ensure documentation is accurate, current, and easy to find
- Reduce onboarding time for new teammates
- Prevent knowledge loss when team members transition

### Typical Communication
- Documentation review comments in PRs and issues
- Quarterly documentation health check shared with Project Manager and Product Manager
- Change requests filed as GitHub Issues when documentation gaps are identified

### Interactions with Other Roles
- **Developers**: Reviews technical PRs for documentation impact; writes or reviews runbooks and API docs
- **Product Managers**: Keeps feature documentation aligned with product decisions and release notes
- **QA Engineers**: Documents test procedures and QA processes
- **Release Manager**: Updates release runbooks and deployment guides after each release cycle
- **Customer Support**: Maintains user-facing guides and FAQs based on common support issues
- **UX/UI Designers**: Documents design system components and usage guidelines

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For ownership and accountability across project lifecycle phases, see [Roles & Responsibility Matrix](./octoacme-roles-responsibility-matrix.md).

