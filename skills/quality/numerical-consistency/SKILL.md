---
name: numerical-consistency
description: Detect inconsistent numbers, units, percentages, totals, and quantitative references within a document.
version: 0.1.0
status: experimental
category: quality
mode: audit
---
# Numerical Consistency

Extract quantitative statements, units, totals, percentages, dates, and repeated values. Compare them across locations and flag mismatches. Recalculate only when the required inputs are present.

Quality gates: expose calculations and assumptions; do not silently correct unknown values.