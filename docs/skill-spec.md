# Skill Specification

Every skill lives at `skills/<domain>/<skill-name>/SKILL.md`.

## Required front matter
```yaml
---
name: example-skill
description: One-sentence trigger description.
version: 0.1.0
status: experimental
category: editing
mode: detect-and-explain
---
```

## Required sections
- Purpose
- When to use
- Inputs
- Procedure
- Constraints
- Output contract
- Failure modes
- Quality gates

## Recommended sections
- Non-goals
- Examples
- Evidence requirements
- Severity model
- Related skills

## Modes
`detect`, `explain`, `suggest`, `rewrite`, `transform`, `verify`, and `audit` may be combined when the skill genuinely supports them.

## Standard severity
`critical`, `high`, `medium`, `low`, `suggestion`.

A skill should prefer findings over silent edits unless the caller explicitly requests transformation.