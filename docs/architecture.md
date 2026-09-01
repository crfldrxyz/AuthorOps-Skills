# AuthorOps-Skills Architecture

## System boundary

AuthorOps-Skills is the **portable skill layer** in a larger AuthorOps ecosystem. It provides reusable intellectual operations. It does not own workflow orchestration.

```text
AUTHOR / RESEARCHER
        |
        v
     AGENT
        |
        v
 AUTHOROPS-SKILLS
   |          |
   v          v
 SKILL     SKILL RESULT
   |          |
   +----------+
        |
        v
 external agent / workflow / application
```

## Design laws
1. **Skill independence:** a skill can be invoked without requiring a particular pipeline.
2. **Composability:** outputs are explicit enough for another skill or agent to consume.
3. **Evidence honesty:** detection is not verification unless evidence supports verification.
4. **Author agency:** preserve meaning, intent, and ownership; do not rewrite by default.
5. **Progressive growth:** add capabilities in response to real work and observed failure modes.
6. **Tool neutrality:** skills may describe optional tools, but their intellectual procedure is not coupled to one vendor.

## Layers
- Domain taxonomy: where a skill belongs.
- Skill contract: what every skill promises.
- Registry: machine-readable discovery metadata.
- Evaluation: examples and regression fixtures maintained with skills.

Pipelines, agents, APIs, applications, and service integrations are intentionally out of scope.