# Task Template

Copy this template when creating new tasks.

---

```markdown
### TASK-XXX: [Action Verb] [Description]
**Priority:** High | Medium | Low
**Assignee:** @Kyrian | @Ivan | @Jonathan
**Status:** To Do
**Effort:** X hours
**Dependencies:** TASK-XXX | None
**Epic:** EPIC-XXX (optional)
**Story:** STORY-XXX (optional)

[Detailed description. Must start with an action verb per Rule 2.]

**Acceptance Criteria:**
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

**Notes:**
- Additional context
- Related links
```

---

## Field Definitions

| Field | Description | Required |
|-------|-------------|----------|
| ID | Unique identifier (TASK-001 format) per Rule 1 | Yes |
| Title | Action verb + description per Rule 2 | Yes |
| Priority | High/Medium/Low per Rule 3 | Yes |
| Assignee | @Kyrian, @Ivan, or @Jonathan per Rule 21 | Yes |
| Status | To Do/In Progress/Review/Done/Blocked/Outdated per Rule 5 | Yes |
| Effort | Hours or days per Rule 4 | Yes |
| Dependencies | Explicit per Rule 7 | Yes |
| Epic | Parent epic if applicable | No |
| Story | Parent story if applicable | No |
| Acceptance Criteria | Checkboxes for completion | Yes |

## Priority Guidelines (Rule 3)

- **High (Red):** Urgent or blocks others
- **Medium (Yellow):** Important but not urgent
- **Low (Green):** Enhancements, nice-to-have

## Status Flow (Rule 5)

```
To Do → In Progress → Review → Done
          ↓
       Blocked → (resolved) → In Progress
          ↓
       Outdated (if no longer needed)
```
