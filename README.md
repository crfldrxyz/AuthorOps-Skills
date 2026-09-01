# AuthorAgent-Skills

An agent-native, composable skills library for serious writing, research, manuscripts, papers, books, editing, citations, and publication-quality review.

## Principle

This repository contains **skills only** as reusable intellectual operations. Skills are designed to work independently or be composed by external agents and workflows.

## Architecture

- `skills/` — canonical skills
- `skills/<domain>/<skill>/SKILL.md` — one independently invocable skill
- `docs/` — repository-level standards and architecture
- `tests/` — evaluation fixtures and regression cases

Each skill follows a common contract: objective, applicability, inputs, procedure, constraints, output, and quality gates.

## Domains

writing · editing · research · citations · academic · manuscripts · books · publishing · quality · forensics

## Evolution

The library is intentionally empirical: skills are improved through real use, evaluation, and observed failure modes. Avoid premature coupling between individual skills.
