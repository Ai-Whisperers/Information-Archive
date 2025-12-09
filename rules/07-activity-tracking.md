# Activity Tracking and Prioritization Rules (61-70)

## Rule 61: Commit-Based Activity Tracking
Track project activity by commit frequency:
- **Active**: Commits within last 7 days
- **Recent**: Commits within last 30 days
- **Semi-Active**: Commits within last 60 days
- **Dormant**: No commits in 60+ days

Review activity status weekly and update project priorities accordingly.

## Rule 62: Owner Assignment by Commit History
Assign project ownership based on commit patterns:
- Primary owner = most commits in last 90 days
- If no commits in 90 days, ownership defaults to @Jonathan (CTO)
- Ownership changes require documented handoff

**Current Ownership Map:**
| Owner | Domains |
|-------|---------|
| @Jonathan | Backend, infrastructure, client sites, tools |
| @Kyrian | Marketing, courses, content, strategy |
| @Ivan | Scrapers, analyzers, automation, internal tools |

## Rule 63: Workload Balancing Threshold
No team member should own more than 60% of active projects:
- If exceeded, redistribute or deprioritize projects
- Track via weekly workload report
- Escalate imbalances in standup

**Current Limits:**
- @Jonathan: Max 6 active projects
- @Kyrian: Max 4 active projects
- @Ivan: Max 4 active projects

## Rule 64: Client Project Priority
Client projects always take priority over internal projects:
- Active client work = High priority automatically
- Client deadlines override internal roadmap
- Document client status in project README

**Client Project Indicators:**
- External stakeholder dependency
- Revenue-generating deliverable
- Contractual obligation

## Rule 65: Dormant Project Review Cadence
Review dormant projects (60+ days inactive) monthly:
1. Check if project is still needed
2. Decide: Archive, Activate, or Keep dormant
3. Update inventory with decision
4. If activating, assign owner and create activation task

## Rule 66: Cross-Project Dependency Mapping
Document dependencies between projects:
- Input/output relationships
- Shared data or APIs
- Deployment dependencies

Update dependency map when:
- New project created
- Integration added
- Project archived

## Rule 67: Priority Calculation Formula
Calculate task priority score using:

```
Priority = (Client Factor × 3) + (Blocker Factor × 2) + (Activity Score × 1)

Where:
- Client Factor: 1 if client project, 0 if internal
- Blocker Factor: 1 if blocks other work, 0 if standalone
- Activity Score: 1 if active, 0.5 if recent, 0.25 if semi-active, 0 if dormant
```

Maximum score: 6 (client + blocker + active)

## Rule 68: Commit Message Standards
All commits should follow conventional commits:
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation only
- `refactor:` Code restructure
- `test:` Test additions
- `chore:` Maintenance tasks

Include ticket ID when applicable: `feat(TASK-011): Add feature`

## Rule 69: Weekly Activity Report
Generate weekly activity report containing:
- Commits by team member
- Projects touched
- Tasks completed
- Blockers encountered
- Next week priorities

Review in Monday standup.

## Rule 70: Project Health Indicators
Monitor project health via:

| Indicator | Healthy | Warning | Critical |
|-----------|---------|---------|----------|
| Days since commit | < 7 | 7-30 | > 30 |
| Open issues | < 5 | 5-15 | > 15 |
| Failing CI | 0 | 1-2 | > 2 |
| Missing docs | None | README only | No README |

Projects with 2+ critical indicators require immediate attention.
