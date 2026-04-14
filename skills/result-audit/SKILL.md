---
name: result-audit
description: Use when an operator must review outputs for unsupported conclusions, weak evidence, missing ablations, broken assumptions, or incomplete reporting.
---

# Result Audit

## When to Use This Skill

Use this skill when the node needs to:

- review a report, notebook, or artifact bundle
- detect unsupported conclusions
- check whether the evidence matches the claimed contribution
- flag missing baselines, controls, or ablations
- judge whether the final output is ready for handoff or publication

## Workflow

1. Read the stated claim before the evidence.
2. Map each important claim to the supporting artifact or result.
3. Check for missing comparisons, controls, or caveats.
4. Identify where the output overstates certainty.
5. Return findings as prioritized review items.

## Expected Outputs

- a severity-ranked review list
- unsupported claim flags
- missing evidence or baseline flags
- final release recommendation

## Quality Rules

- focus on evidence, not writing style
- do not accept "looks plausible" as support
- call out missing baselines explicitly
- separate hard failures from optional improvements
