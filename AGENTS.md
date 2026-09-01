# AuthorOps-Skills Agent Guidance

AuthorOps-Skills is a portable, standalone skill library. Treat every `skills/**/SKILL.md` as an independently invocable intellectual operation.

## Boundaries
- This repository contains skills and the standards needed to make skills interoperable.
- Do not add workflow orchestration, application code, vendor-specific agent implementations, or UI.
- Prefer small composable skills over giant all-purpose prompts.
- Skills detect, explain, suggest, rewrite, verify, or audit; they should state which mode they support.
- Never claim external verification, plagiarism detection, citation validation, or source access unless the required evidence/tool is actually available.
- Preserve author intent and agency. Default to identifying and explaining problems before rewriting.

## Skill quality
A skill must have: precise purpose, explicit applicability, inputs, procedure, constraints, output contract, failure modes, and quality gates.

## Evolution
Improve skills from real use and observed failures. New behavior should be backed by examples or regression cases when practical.
