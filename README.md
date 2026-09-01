# AuthorAgent-Skills

An agent-native, composable skills library for serious writing, research, manuscripts, papers, books, editing, citations, and publication-quality review.

## Principle

This repository contains **skills, not applications or pipelines**. Each skill is an independently usable intellectual operation that external agents and future workflow systems can compose.

## Skill Contract

Every canonical skill lives at `skills/<domain>/<skill>/SKILL.md` and defines:

- objective and scope
- when to use it
- expected inputs
- operational procedure
- constraints and failure boundaries
- output contract
- quality gates
- confidence expectations

Skills diagnose before rewriting whenever practical, preserve author intent, and never fabricate evidence, citations, source support, or verification results.

## Domains

- `writing` — composition, structure, paragraphs, transitions, argument development
- `editing` — grammar, proofreading, clarity, concision, readability, mechanics
- `style` — voice, tone, register, active/passive voice
- `transformation` — paraphrasing and meaning-preserving revision
- `research` — questions, literature, sources, evidence, research reasoning
- `citations` — generation, completeness, validation, source-to-claim traceability
- `academic` — papers, abstracts, methodology, scholarly conventions
- `quality` — coherence, consistency, terminology, redundancy and final quality controls
- `forensics` — claim audits, overclaiming, plagiarism risk and evidence integrity
- `reasoning` — argument reconstruction and logical analysis

## Current Foundation

The initial library establishes 33 reusable skills spanning surface editing through research and evidentiary integrity. This is a living foundation, not a frozen taxonomy.

## Evolution Model

Real documents are the test environment. When a skill fails, the failure becomes a candidate improvement, regression case, or new skill. Skills should remain independently evolvable; composition belongs to agents and external workflow layers.

## Non-Goals

This repository does not pretend that a markdown skill can replace external plagiarism corpora, scholarly databases, citation metadata services, domain experts, or human editorial judgment. Where external verification is required, the skill must say so explicitly.
