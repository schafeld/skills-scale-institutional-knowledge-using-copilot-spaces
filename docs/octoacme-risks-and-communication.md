# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

### Sample Risk Register

| ID | Description | Impact | Likelihood | Owner | Mitigation Plan | Status |
|----|-------------|--------|------------|-------|-----------------|--------|
| R-001 | Third-party API dependency may have downtime during peak usage | High | Medium | Lead Developer | Implement retry logic and fallback mechanism; monitor API health | Active |
| R-002 | UX design timeline may delay feature development | Medium | Low | UX Designer | Begin design work in parallel with planning; get early stakeholder feedback | Mitigated |
| R-003 | Security review may identify vulnerabilities requiring refactoring | High | Medium | Security Lead | Schedule security review early in development; allocate buffer time | Active |

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, executive sponsors)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Tailor communication to audience: executives need high-level summaries, technical teams need details

### Stakeholder Communication Matrix

| Stakeholder Group | Primary Contact | Frequency | Method | Content Focus |
|-------------------|----------------|-----------|---------|---------------|
| Executive Sponsor | Project Manager | Monthly | Email summary + meeting | Business impact, risks, key decisions |
| Product Leadership | Product Manager | Weekly | Sync meeting | Progress, priorities, trade-offs |
| Development Team | Project Manager | Daily/Weekly | Standup + Slack | Tasks, blockers, technical details |
| UX/Design Team | UX Designer | Weekly | Design review | User research, prototypes, feedback |
| Security Team | Security Lead | Milestone-based | Review meeting | Threat assessment, vulnerabilities, compliance |
| Technical Writing | Technical Writer | Weekly | Sync + doc reviews | Release notes, user guides, API docs |
| Customer Support | Project Manager | Before release | Email + training | New features, changes, known issues |

## Communication Templates

### Weekly Status Template:
**To:** [Stakeholder group]  
**From:** [Project Manager name]  
**Subject:** [Project Name] - Weekly Update [Date]

**Progress this week:**
- [Key accomplishment 1]
- [Key accomplishment 2]
- [Milestone reached or upcoming]

**Next steps:**
- [Planned work for next week]
- [Key decisions or meetings scheduled]

**Risks & blockers:**
- [Active risks from risk register]
- [Blockers requiring escalation or help]

**Ask / decisions needed:**
- [Specific requests or decisions needed from stakeholders]
- [Resource needs or approvals required]

**Team Status:**
- Developers: [Brief status]
- UX Designer: [Brief status]
- Technical Writer: [Brief status]
- Security Lead: [Brief status]

---

### Stakeholder Update for Executive Sponsors

**To:** [Executive Sponsor name]  
**From:** [Project Manager name]  
**Subject:** [Project Name] - Monthly Executive Update [Month]

**Executive Summary:**
[2-3 sentence overview of project status and key highlights]

**Progress Against Goals:**
- Success Metric 1: [Current status vs. target]
- Success Metric 2: [Current status vs. target]
- Timeline: [On track / At risk / Delayed - brief explanation]
- Budget: [Within budget / Over budget - brief explanation]

**Key Accomplishments:**
- [Major milestone or achievement]
- [Significant feature delivery or progress]

**Top Risks:**
- [Risk 1 - Impact, mitigation plan, owner]
- [Risk 2 - Impact, mitigation plan, owner]

**Decisions Needed:**
- [Decision 1 - Context, options, recommendation, by when]
- [Decision 2 - Context, options, recommendation, by when]

**Next Milestone:**
[Upcoming milestone, date, key deliverables]

---

### Escalation Communication Template

**To:** [Manager or Sponsor name]  
**From:** [Project Manager name]  
**Subject:** ESCALATION: [Project Name] - [Brief issue description]  
**Priority:** [High / Critical]

**Issue Summary:**
[Clear description of the problem or blocker]

**Impact:**
- Business impact: [How this affects project goals, timeline, or customers]
- Timeline impact: [Days/weeks of potential delay]
- Affected stakeholders: [Who is impacted]

**Current Status:**
[What has been tried so far to resolve the issue]

**Assistance Needed:**
[Specific help or decision required from the recipient]
- Option 1: [Description, pros/cons]
- Option 2: [Description, pros/cons]
- Recommended: [Your recommendation]

**Response Needed By:**
[Date and time by which decision is needed]

**Escalation Owner:**
[Name and role of person managing this escalation]

---

### Incident Communication

**Incident ID:** [ID number]  
**Severity:** [Critical / High / Medium / Low]  
**Status:** [Investigating / Mitigating / Resolved]

**Summary:**
[Brief description of the incident]

**Impact:**
- Affected services/features: [List]
- User impact: [Description]
- Started at: [Timestamp]

**Actions being taken:**
- [Action 1 - Owner, status]
- [Action 2 - Owner, status]

**Expected timeline:**
[When resolution is expected or next update will be provided]

**Communication plan:**
- Next update: [When]
- Stakeholders notified: [List]
- Customer communication: [Status or plan]

**Post-incident review:**
- Scheduled for: [Date]
- Format: Blameless retrospective
- Attendees: [PM, relevant developers, Security Lead if applicable]

## Escalation Paths

### Standard Escalation Hierarchy
**Level 1: Team-level resolution**
- Who: Development team, Project Manager
- Timeline: Resolve within 1-2 days
- Examples: Technical blockers, clarification on requirements, minor scope questions

**Level 2: Product/Project Leadership**
- Who: Product Manager, Engineering Lead
- Escalated by: Project Manager
- Timeline: Resolve within 2-3 days
- Examples: Cross-team dependencies, resource constraints, scope trade-offs, medium risks

**Level 3: Executive/Sponsor**
- Who: Executive Sponsor, Department Head
- Escalated by: Product Manager or Project Manager
- Timeline: Resolve within 1 week
- Examples: Major scope changes, budget increases, critical risks, strategic decisions

### Role-Specific Escalation Paths

**Security Incidents:**
- Immediate: Security Lead → Security On-call
- Critical: Security Lead → CISO → Executive team
- Follow security incident runbook for detailed procedures

**UX/Design Issues:**
- Level 1: UX Designer → Product Manager
- Level 2: Product Manager → Design Lead
- Level 3: Design Lead → Product Leadership

**Documentation Issues:**
- Level 1: Technical Writer → Project Manager
- Level 2: Project Manager → Documentation Lead
- For release-blocking docs: Immediate escalation to Product Manager

**Quality/Testing Issues:**
- Level 1: QA → Development team
- Level 2: Project Manager → Engineering Lead
- For release-blocking issues: Immediate escalation to Product Manager

### Escalation Guidelines
- **When to escalate:** When a blocker cannot be resolved at the current level within the timeline shown above, or when a decision requires authority beyond the current level
- **How to escalate:** Use the escalation communication template (see Communication Templates section)
- **Follow-up:** Escalating party owns tracking the issue to resolution and communicating outcome back to the team
