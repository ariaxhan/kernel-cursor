---
description: Generate a structured context handoff brief for seamless conversation continuation
---

# Context Handoff

Generate a token-optimized brief that enables seamless conversation continuation.

## When to Use

- Need to transfer conversation to another session
- Need to pause work and resume later
- Switching between AI tools

## Step 1: Extract Current State

Gather:
- **Goal**: What is the user trying to achieve?
- **Position**: Where are we in the workflow?
- **Decisions**: What choices were made and why?
- **Open Threads**: What's unfinished or unresolved?
- **Artifacts**: What was created (files, code, frameworks)?
- **Warnings**: Failed approaches, pitfalls to avoid

## Step 2: Check Recent Work

```bash
git status --short
git log --oneline -5
```

## Step 3: Generate Handoff

```
## CONTEXT HANDOFF

**Summary**: [One sentence capturing entire situation]

**Goal**: [What user is trying to achieve]

**Current state**: [Where things stand now - concrete, specific]

**Decisions made**:
- [Decision 1: choice + rationale]
- [Decision 2]

**Artifacts created**:
- [File/framework 1 with path]
- [File/framework 2 with path]

**Open threads**:
- [Unfinished item 1]
- [Question needing resolution]

**Next steps**:
1. [Recommended action 1 - specific, actionable]
2. [Recommended action 2]

**Warnings**:
- [Pitfall/failed approach to avoid]

**File paths to read**:
- [Key file 1]
- [Key file 2]

**Continuation prompt**:
> [2-3 sentences: goal, current position, next action]
```

## Compression Rules

- **One sentence max per bullet**
- **No redundancy** between sections
- **Omit empty sections**
- **Actionable over descriptive**
- **Concrete over vague**

Present the handoff in a code block for easy copy-paste.
