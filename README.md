# AuthorOps-Skills

Portable, agent-native skills for serious writing, research, editing, citations, manuscripts, books, academic work, and publication-quality review.

**AuthorOps-Skills is the skill layer only.** It contains independently invocable `SKILL.md` units plus the standards needed to make them discoverable, testable, evidence-aware, and interoperable. End-to-end pipelines, workflow orchestration, product code, and vendor-specific agent implementations belong outside this repository.

## Core idea

> Build reusable intellectual operations first; let real work reveal the architecture that comes next.

The library is designed to grow empirically through real documents, evaluation, observed failure modes, and focused revisions. Skills stay small enough to compose and explicit enough for agents to invoke independently.

## Current coverage

The initial library contains **85 registered skills** across 11 domains:

`writing` · `editing` · `transformation` · `research` · `citations` · `academic` · `manuscripts` · `books` · `publishing` · `quality` · `forensics`

Coverage includes grammar, proofreading, spelling, punctuation, clarity, concision, coherence, redundancy, active/passive voice, paraphrasing, meaning preservation, simplification, formalization, source and evidence work, citation generation/checking, academic-paper review, manuscript and book structure, publication readiness, reasoning quality, plagiarism-risk review, quotation integrity, provenance, and final document audit.

## Architecture

```text
skills/<domain>/<skill-name>/SKILL.md
                │
                ├── common skill contract
                ├── bounded procedure
                ├── evidence constraints
                ├── structured output
                └── quality gates
                         │
                         ▼
                external agent / workflow
```

The repository deliberately does **not** define pipelines. A future AuthorOps pipeline layer may consume these skills without changing their ownership or independence.

## Canonical references

- `docs/skill-spec.md` — required skill structure and metadata.
- `docs/output-contract.md` — structured result conventions.
- `docs/evidence-policy.md` — verification and provenance boundaries.
- `docs/evaluation.md` — evaluation and regression philosophy.
- `registry/skills.yaml` — machine-readable discovery index.
