# Kernel for Cursor

**The Complete AI Coding OS for Cursor.**

7 @-mentionable agents | 10 methodology banks | 4 project-notes | session memory

---

## Quick Install

1. Copy `.cursor/rules/` to your project
2. Copy `kernel/` and `_meta/` to your project
3. Done - rules load automatically

```
your-project/
├── .cursor/
│   └── rules/           <-- Cursor auto-loads these
│       ├── kernel-core.mdc
│       ├── agent-debugger.mdc
│       ├── agent-reviewer.mdc
│       ├── agent-planner.mdc
│       ├── agent-tester.mdc
│       ├── agent-security.mdc
│       ├── agent-refactor.mdc
│       └── agent-shipper.mdc
├── kernel/
│   ├── banks/           <-- 10 methodology templates
│   ├── project-notes/   <-- 4 memory templates
│   └── state.md
└── _meta/               <-- Session tracking
```

---

## Usage

### @-Mention Agents

Type `@` followed by the agent name:

| Agent | When to Use |
|-------|-------------|
| `@debugger` | Stuck on a bug |
| `@reviewer` | Before shipping code |
| `@planner` | Starting a non-trivial feature |
| `@tester` | After writing code |
| `@security` | Auth, input handling, pre-ship |
| `@refactor` | Code needs cleanup |
| `@shipper` | Ready to commit/push/PR |

### Project Notes (Check FIRST)

Before debugging or deciding, check:
- `kernel/project-notes/bugs.md` - Past bug solutions
- `kernel/project-notes/decisions.md` - Architecture decisions
- `kernel/project-notes/key_facts.md` - Infrastructure knowledge
- `kernel/project-notes/issues.md` - Work log

### Methodology Banks

In `kernel/banks/` - load when needed:
- `DEBUGGING-BANK.md` - Deep debugging methodology
- `PLANNING-BANK.md` - Feature planning
- `REVIEW-BANK.md` - Code review checklist
- And 7 more...

---

## Self-Evolution

When you learn something:
1. Log to `_meta/_learnings.md`
2. Update the relevant rule
3. The system gets smarter

---

## Differences from Claude Code Version

| Feature | Claude Code | Cursor |
|---------|-------------|--------|
| Agents | 19 (Task tool) | 7 (@-mentionable rules) |
| Rules | 12 (.md files) | 8 (.mdc files) |
| Commands | 14 (slash commands) | Via agents |
| Format | Markdown | MDC with YAML frontmatter |

Same philosophy. Same project-notes. Same methodology banks. Different interface.

---

Built for Cursor users who want AI that actually learns their codebase.
