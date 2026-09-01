---
name: proofreading
description: Perform final surface-level review for spelling, punctuation, typographic consistency, formatting anomalies, and obvious language errors without changing substantive meaning.
metadata:
  category: editing
  maturity: core
  version: "0.1.0"
---
# Proofreading

Review from the smallest surface unit upward: word, sentence, paragraph, document. Detect errors, preserve intentional style, and report rather than silently altering content.

## Checks
- spelling and capitalization
- punctuation and quotation marks
- spacing and typography
- repeated or missing words
- inconsistent formatting
- obvious grammar defects

## Output
Return findings with location, original, correction, reason, and confidence. Separate mandatory corrections from optional style suggestions.

## Quality Gate
Do not introduce factual, stylistic, or substantive changes under the label of proofreading.
