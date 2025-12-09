# Templates

Standardized templates for project documentation.

## Available Templates

| Template | Use Case | Rules Referenced |
|----------|----------|------------------|
| [task-template.md](task-template.md) | Creating new tasks | Rules 1-10 |
| [story-template.md](story-template.md) | Creating user stories | Rules 11-20 |
| [epic-template.md](epic-template.md) | Creating epics | Rules 11, 19, 20 |

## How to Use

1. Navigate to the appropriate template
2. Copy the markdown content
3. Paste into the target document
4. Fill in the placeholders
5. Remove any sections not needed

## Template Standards

All templates follow these conventions:

- **IDs:** Unique alphanumeric (EPIC-001, STORY-001, TASK-001)
- **Descriptions:** Start with action verbs
- **Priorities:** High (Red), Medium (Yellow), Low (Green)
- **Status:** To Do → In Progress → Review → Done | Blocked | Outdated
- **Assignees:** @Kyrian, @Ivan, @Jonathan only

## Adding New Templates

When creating a new template:

1. Follow existing naming convention (`[type]-template.md`)
2. Include field definitions table
3. Reference applicable rules
4. Add to this README
5. Update INDEX.md
