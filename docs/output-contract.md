# Output Contract

Skills should produce structured, predictable results when the caller requests machine-readable output.

```yaml
skill: clarity-check
status: completed
summary: Short overall assessment.
findings:
  - id: CL-001
    severity: high
    location: paragraph 4, sentence 2
    issue: ambiguous-reference
    evidence: The word "this" has no clear antecedent.
    recommendation: Name the concept explicitly.
    confidence: 0.94
```

## Rules
- `evidence` describes observable text or available source evidence.
- `confidence` reflects uncertainty in the skill's judgment, not factual truth.
- Never fabricate source data, citations, quotations, or verification.
- `rewrite` output must be separable from the finding so callers can choose whether to apply it.
- A skill may return `not-verifiable` when required evidence or tool access is unavailable.