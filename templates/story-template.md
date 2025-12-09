# Story Template

Copy this template when creating new user stories.

---

```markdown
### STORY-XXX: [Title]
**Epic:** EPIC-XXX
**Priority:** High | Medium | Low
**Status:** To Do
**Assignee:** @Kyrian | @Ivan | @Jonathan

**User Story:**
As a [role], I want [feature/capability] so that [benefit/value].

**Acceptance Criteria:**
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

**Tasks:**
- [ ] TASK-XXX: [Description]
- [ ] TASK-XXX: [Description]
- [ ] TASK-XXX: [Description]

**Notes:**
- Additional context
- Design considerations
- Related stories
```

---

## Field Definitions

| Field | Description | Required |
|-------|-------------|----------|
| ID | Unique identifier (STORY-001 format) | Yes |
| Title | Brief descriptive title | Yes |
| Epic | Parent epic reference | Yes |
| Priority | High/Medium/Low | Yes |
| Status | To Do/In Progress/Done | Yes |
| Assignee | Primary owner | Yes |
| User Story | "As a... I want... so that..." per Rule 12 | Yes |
| Acceptance Criteria | Checkboxes per Rule 20 | Yes |
| Tasks | 5-8 tasks per Rule 13 | Yes |

## Story Format (Rule 12)

Stories must be phrased as:
> "As a [role], I want [feature] so that [benefit]."

**Examples:**
- "As a developer, I want to filter inactive repos so that I can focus on active work."
- "As a PM, I want to see task dependencies so that I can plan sprints."
- "As a client, I want real-time feedback so that I can improve quickly."

## Task Breakdown (Rules 13-14)

- Limit to 5-8 tasks per story
- Each task should have 3-7 subtasks
- Subtasks must be completable in < 4 hours
