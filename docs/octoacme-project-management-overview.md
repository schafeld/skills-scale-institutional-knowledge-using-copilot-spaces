# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Developers: implement features, collaborate on design and testability.
- UX Designer: creates user-friendly interfaces and validates usability.
- Technical Writer: maintains clear, accurate documentation for users and developers.
- Security Lead: ensures security best practices and identifies vulnerabilities.
- QA/Testing: validate quality and acceptance criteria.
- Stakeholders/Sponsors: provide strategic direction, funding, and approvals.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence

### Regular Sync Meetings
- **Daily standups** (15 min): Development team shares progress, blockers, and daily priorities
- **Weekly PM + PdM sync**: Align on priorities, review risks, discuss stakeholder feedback
- **Twice-weekly delivery team standups** (or as agreed): Full team including UX, Technical Writer, and Security Lead when relevant
- **Weekly status updates**: PM sends written updates to stakeholders (see Communication Templates in Risk & Communication doc)
- **Monthly stakeholder reviews**: Executive-level updates on progress, metrics, and key decisions
- **Sprint/Milestone demos**: Show working software to stakeholders and gather feedback

### Ad-hoc Communication
- **Escalations**: Follow the escalation paths defined in the Risk & Communication document
- **Blocker resolution**: Immediate communication when critical issues arise
- **Design reviews**: Scheduled by UX Designer as needed for feedback
- **Security reviews**: Scheduled by Security Lead at key milestones
- **Documentation reviews**: Technical Writer coordinates with developers before releases

### Artifact Updates and Maintenance
Keeping project artifacts current is essential for alignment and decision-making:

- **Project Charter/One-pager**: Update when scope, timeline, or success metrics change (PM owns)
- **Risk Register**: Review and update weekly during PM/PdM sync (PM owns)
- **Backlog**: Prioritize and refine continuously; formal review in sprint planning (PdM owns)
- **Release Plan**: Update when milestones shift or dependencies change (PM owns)
- **Communication Plan**: Review monthly to ensure stakeholder needs are met (PM owns)
- **Documentation**: Update with each feature delivery (Technical Writer owns, Developers contribute)
- **Retrospective Action Items**: Track in project board and review status weekly (PM facilitates, team owns)

### Escalation Paths
When issues cannot be resolved at the team level:
1. **Team-level**: Development team and PM resolve technical blockers (1-2 days)
2. **Product/Project Leadership**: PM escalates to Product Manager or Engineering Lead for cross-team issues or resource needs (2-3 days)
3. **Executive/Sponsor**: PM or PdM escalates to Executive Sponsor for strategic decisions, major scope changes, or critical risks (up to 1 week)

Special escalation paths exist for:
- **Security incidents**: Security Lead → Security On-call → CISO (immediate)
- **Release-blocking issues**: PM → Product Manager (immediate)

See the [Risk & Communication document](octoacme-risks-and-communication.md) for detailed escalation templates and procedures.

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
