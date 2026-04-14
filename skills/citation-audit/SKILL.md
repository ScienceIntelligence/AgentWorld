---
name: citation-audit
description: Use when an operator must verify citation accuracy, bibliography consistency, metadata quality, and whether claims are actually supported by the cited sources.
---

# Citation Audit

## When to Use This Skill

Use this skill when the node needs to:

- verify that citations support the written claim
- check metadata such as title, authors, venue, year, and DOI
- detect missing or duplicate references
- clean up a bibliography before release
- review whether a writeup overstates what a cited paper proves

## Workflow

1. Check whether every major claim has a citation.
2. For each citation, confirm that the source actually supports the stated claim.
3. Normalize key metadata fields.
4. Remove duplicates and weak citations.
5. Flag unsupported or overstated claims.

## Expected Outputs

- a citation issue list
- corrected metadata suggestions
- unsupported claim warnings
- a cleaned bibliography checklist

## Quality Rules

- citation presence is not enough; support must be real
- prefer primary papers over derivative references
- flag ambiguous or second-hand citations
- keep corrections explicit and actionable
