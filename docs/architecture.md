# AuthorOps-Skills Architecture

## System boundary

AuthorOps-Skills is a **standalone portable skill library**. It defines reusable intellectual operations and the standards required to describe, discover, evaluate, and invoke them. It has no dependency on a separate orchestration layer, application, vendor, or service.

```text
AUTHOR / RESEARCHER
        |
        v
     AGENT
        |
        v
 AUTHOROPS-SKILLS
        |
        v
      SKILL
        |
        v
   SKILL RESULT
```

## Design laws
1. **Skill independence:** every skill can be invoked without requiring another repository or system.
2. **Composability:** outputs are explicit enough for a caller to consume.
3. **Evidence honesty:** detection is not verification unless evidence supports verification.
4. **Author agency:** preserve meaning, intent, and ownership; do not rewrite by default.
5. **Progressive growth:** add capabilities in response to real work and observed failure modes.
6. **Tool neutrality:** skills may describe optional tools, but their intellectual procedure is not coupled to one vendor.
7. **Repository independence:** the skill library must remain useful and complete on its own.

## Layers
- Domain taxonomy: where a skill belongs.
- Skill contract: what every skill promises.
- Registry: machine-readable discovery metadata.
- Evaluation: examples and regression fixtures maintained with skills.

Workflow orchestration, agents, APIs, applications, and service integrations are outside the repository boundary. They may consume a skill, but they are not part of this repository's architecture or ownership.
