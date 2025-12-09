# Contributing to Information-Archive

Thank you for contributing to the Repository Dashboard project!

## Quick Start

1. Clone the repository
2. Create a branch for your changes
3. Make your changes following the guidelines below
4. Submit a pull request

## Branch Naming Convention

Use descriptive branch names:
- `feat/description` - New features
- `fix/description` - Bug fixes
- `docs/description` - Documentation changes
- `refactor/description` - Code restructuring

## Commit Message Format

Follow conventional commits (Rule 68):

```
type(scope): description

[optional body]

[optional footer]
```

**Types:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation only
- `refactor:` Code restructure
- `test:` Test additions
- `chore:` Maintenance tasks

**Examples:**
```
feat(TASK-011): Add website consolidation plan
docs: Update repository inventory with new descriptions
fix(EPIC-002): Correct marketing pipeline dependencies
```

## Task Creation

When creating new tasks, follow this template:

```markdown
### TASK-XXX: [Action verb] [Description]
**Priority:** High | Medium | Low
**Assignee:** @Kyrian | @Ivan | @Jonathan
**Status:** To Do
**Effort:** X hours
**Dependencies:** TASK-XXX or None

[Detailed description starting with a verb]

**Acceptance Criteria:**
- [ ] Criterion 1
- [ ] Criterion 2
```

## Story Creation

Stories follow Rule 12 format:

```markdown
### STORY-XXX: [Title]
**Epic:** EPIC-XXX
**Priority:** High | Medium | Low
**Assignee:** @Name

As a [role], I want [feature] so that [benefit].

**Acceptance Criteria:**
- [ ] Criterion 1
- [ ] Criterion 2

**Tasks:**
- TASK-XXX
- TASK-XXX
```

## Pull Request Process

1. Update documentation if needed
2. Add your changes to the relevant task/story
3. Reference task IDs in PR description
4. Request review from the appropriate team member:
   - @Jonathan for technical changes
   - @Kyrian for process/documentation changes
   - @Ivan for tooling/automation changes

## Review Guidelines

Per Rule 35, reviews are required for Done status:

- [ ] Changes follow existing patterns
- [ ] Documentation is updated
- [ ] Links are valid
- [ ] Task IDs are referenced

## Team Assignments

| Area | Lead |
|------|------|
| Backend, Hosting, Architecture | @Jonathan |
| Outreach, PM, Client Investigation | @Kyrian |
| Tools, Scrapers, Automation | @Ivan |

## Questions?

- Technical: @Jonathan
- Process: @Kyrian
- Tooling: @Ivan
