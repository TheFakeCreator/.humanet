# Discussions

This folder contains decision logs, architecture decision records (ADRs), and important discussions.

## 📋 What Goes Here?

### Architecture Decision Records (ADRs)
Document significant architectural or design decisions, including:
- Context and problem
- Decision made
- Alternatives considered
- Consequences

### Design Discussions
- UI/UX decisions
- Feature debates
- Approach comparisons

### Meeting Notes
- Planning meetings
- Brainstorming sessions
- Stakeholder discussions

## 📝 Naming Convention

Use sequential numbering with descriptive names:

```
001-tech-stack-selection.md
002-database-choice.md
003-authentication-strategy.md
004-api-design-approach.md
```

## 📄 ADR Template

Each decision record should follow this structure:

```markdown
# [Number]. [Title]

**Date:** YYYY-MM-DD
**Status:** Proposed | Accepted | Deprecated | Superseded
**Deciders:** [List of people involved]

## Context

[Describe the issue or decision that needs to be made]

## Decision

[State the decision that was made]

## Alternatives Considered

### Option 1: [Name]
- **Pros:** [Benefits]
- **Cons:** [Drawbacks]

### Option 2: [Name]
- **Pros:** [Benefits]
- **Cons:** [Drawbacks]

## Consequences

**Positive:**
- [Benefit 1]
- [Benefit 2]

**Negative:**
- [Tradeoff 1]
- [Tradeoff 2]

**Neutral:**
- [Other consequence]

## References

- [Link to relevant discussion]
- [Related ADR]
```

## 🗂️ Organization

Keep discussions organized and easy to find:

```
discussions/
├── README.md
├── 001-initial-tech-stack.md
├── 002-deployment-strategy.md
├── 003-authentication-approach.md
└── meetings/
    ├── 2026-02-15-kickoff.md
    └── 2026-02-20-planning.md
```

## 🔗 Linking to ADRs

Reference decision records in your main documentation:

```markdown
We chose PostgreSQL for the database (see [ADR-002](./discussions/002-database-choice.md))
```

## ✅ Best Practices

1. **Document decisions when they're made** — Don't wait
2. **Be concise but complete** — Capture enough context
3. **Update status** — Mark decisions as deprecated when superseded
4. **Link related ADRs** — Show decision evolution
5. **Include dates** — Track when decisions were made

---

**Sample decision record is included as an example.**
