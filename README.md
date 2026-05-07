# Cursor Rules
Shared template for managing Cursor rules across team and customers.

This repository separates:
- **General team rules** (applies broadly)
- **Customer/project-specific rules** (applies locally)

---

## Goal

Create a consistent AI-assisted development setup where:

- Team-wide best practices are reused across projects
- Each customer/project can define its own specific rules
- Rules are versioned and reviewed through GitHub PRs

---

## Recommended Rule Strategy

Use a layered approach:

1. **Global / Team rules**  
   Broad, stable guidance (quality, communication style)

2. **Project-specific rules**  
   Concrete implementation details (stack conventions, folder structure, naming, commands)

When there are no conflicts, both layers are used together.  
Keep global rules high-level and project rules specific to avoid overlap.

---

## Repository Structure (Example)

```text
cursor_template/
├── README.md
├── shared/
│   └── .cursor/
│       └── rules/
│           ├── 00-team-core.mdc
├── Lundbeck/
│   ├── .cursor/
│   │   └── rules/
│   │       └── 90-lundbeck-specific.mdc
│   ├── .sqlfluff
│   ├── docs/
│   │   ├── setup.md
│   │   └── guidelines.md
│   └── templates/
