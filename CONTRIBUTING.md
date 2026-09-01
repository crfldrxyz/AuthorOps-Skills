# Contributing

Contributions should improve a real, reusable intellectual operation.

## Add a skill
Create `skills/<domain>/<skill-name>/SKILL.md` using `docs/skill-spec.md`. Keep the skill independently useful, narrowly scoped, and tool-agnostic.

## Naming
Use lowercase kebab-case. Names describe the operation, not a product or model.

## Quality bar
A contribution should define what it checks or changes, what it must not infer, what evidence it needs, and how success is judged. Avoid synonym-swapping presented as paraphrasing, unsupported claims of factual verification, or promises of detector-proof text.

## Changes
Prefer focused commits. Update `registry/skills.yaml` when adding or materially changing a skill. Add regression examples under the skill directory when a failure mode is important enough to preserve.