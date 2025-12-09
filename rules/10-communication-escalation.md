# Rules 91-100: Communication & Escalation

Standards for team communication, client interaction, and issue escalation.

---

## Rule 91: Communication Channels

Use appropriate channels for different purposes:

| Channel | Use For | Response Time |
|---------|---------|---------------|
| Slack/Discord | Quick questions, updates | Same day |
| GitHub Issues | Bug reports, feature requests | 48 hours |
| Email | Client communication, formal | 24 hours |
| Meetings | Complex discussions, planning | Scheduled |

**Never** discuss sensitive data in unencrypted channels.

---

## Rule 92: Status Updates

Provide regular status updates:
- **Daily**: Brief progress in standup channel
- **Weekly**: Summary of completed/blocked items
- **On blockers**: Immediately notify affected parties

**Format:**
```
Done: [What you finished]
Doing: [Current focus]
Blocked: [Issues needing help]
```

---

## Rule 93: Blocker Escalation

Escalate blockers using this timeline:

| Blocker Duration | Action |
|------------------|--------|
| < 2 hours | Self-solve, research |
| 2-4 hours | Ask team for help |
| 4-8 hours | Escalate to lead |
| > 8 hours | Formal blocker review |

**Never** sit on a blocker for more than a day without escalating.

---

## Rule 94: Client Communication

Client-facing communication rules:
- **Response time**: 24 hours max
- **Tone**: Professional, solution-oriented
- **Bad news**: Deliver early with options
- **Scope changes**: Document in writing

**Template for delays:**
```
Hi [Client],

We've encountered [brief issue]. We're actively working on it and expect
resolution by [date].

Options:
1. [Option A]
2. [Option B]

Please let us know your preference.

Best,
[Name]
```

---

## Rule 95: Meeting Efficiency

Meetings MUST be productive:
- **Required**: Agenda sent 24h before
- **Duration**: 30 min default, 60 min max
- **Output**: Action items with owners
- **Record**: Notes in shared doc

**Skip the meeting if:**
- No agenda exists
- Could be an email/message
- Key decision-makers absent

---

## Rule 96: Incident Response

When production issues occur:

| Severity | Response Time | Escalation |
|----------|---------------|------------|
| Critical (down) | 15 min | All hands |
| High (degraded) | 1 hour | On-call + lead |
| Medium (partial) | 4 hours | On-call |
| Low (cosmetic) | 24 hours | Normal ticket |

**Incident process:**
1. Acknowledge incident
2. Assess severity
3. Communicate status
4. Fix or rollback
5. Post-mortem within 48h

---

## Rule 97: Knowledge Sharing

Share knowledge proactively:
- Document solutions to tricky problems
- Share useful tools/techniques in team channel
- Create runbooks for recurring issues
- Pair program on complex features

**Weekly knowledge share:**
- Each team member shares one thing learned
- 5 minutes per person
- Optional but encouraged

---

## Rule 98: Feedback Culture

Provide constructive feedback:
- **Timely**: Within 24h of event
- **Specific**: Cite exact examples
- **Actionable**: Suggest improvements
- **Private**: Criticism in private, praise in public

**Feedback format:**
```
"When you [specific action], it [impact].
Next time, consider [suggestion]."
```

---

## Rule 99: Conflict Resolution

Resolve conflicts professionally:

1. **Step 1**: Direct conversation between parties
2. **Step 2**: Involve neutral team member
3. **Step 3**: Escalate to leadership
4. **Step 4**: Formal mediation if needed

**Ground rules:**
- Focus on issues, not personalities
- Listen before responding
- Seek compromise
- Document agreements

---

## Rule 100: Continuous Improvement

The team continuously improves:
- **Retrospectives**: Monthly, actionable items
- **Process reviews**: Quarterly, update rules
- **Skill development**: Each member learning something new
- **Tool evaluation**: Quarterly, adopt or drop

**This ruleset is a living document.**
Propose changes via PR with justification.
Review and update quarterly.

---

## Quick Reference

| Rule | Topic | Key Point |
|------|-------|-----------|
| 91 | Channels | Right tool for the job |
| 92 | Status | Daily done/doing/blocked |
| 93 | Blockers | Escalate within 4-8 hours |
| 94 | Clients | 24h response, solution-focused |
| 95 | Meetings | Agenda required, 30 min default |
| 96 | Incidents | Severity-based response |
| 97 | Knowledge | Share learnings weekly |
| 98 | Feedback | Specific, timely, actionable |
| 99 | Conflicts | Direct → Neutral → Lead |
| 100 | Improvement | Quarterly process reviews |

---

## Complete Rule Index (1-100)

| Category | Rules | File |
|----------|-------|------|
| Core Task Management | 1-10 | 01-core-task-management.md |
| Hierarchy & Breakdown | 11-20 | 02-hierarchy-breakdown.md |
| Role Assignment | 21-30 | 03-role-assignment.md |
| Workflow Cadence | 31-40 | 04-workflow-cadence.md |
| Dashboard Integration | 41-50 | 05-dashboard-integration.md |
| Repository Standards | 51-60 | 06-repository-standards.md |
| Activity Tracking | 61-70 | 07-activity-tracking.md |
| Documentation Standards | 71-80 | 08-documentation-standards.md |
| Quality & Testing | 81-90 | 09-quality-testing.md |
| Communication & Escalation | 91-100 | 10-communication-escalation.md |

**Total: 100 Rules**
