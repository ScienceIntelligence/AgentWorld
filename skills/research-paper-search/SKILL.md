---
name: research-paper-search
description: Use when an operator needs to find relevant papers, databases, identifiers, benchmark references, or primary-source evidence before planning or implementation.
---

# Research Paper Search

## When to Use This Skill

Use this skill when the node needs to:

- find primary papers for a topic
- identify canonical baselines or benchmark papers
- collect DOI, arXiv, PMID, or project URLs
- narrow a broad problem into a tractable evidence set
- distinguish primary sources from commentary or summaries

## Workflow

1. Start from the task objective and convert it into 2-4 search queries.
2. Prefer primary sources: papers, official datasets, benchmark repos, and technical documentation.
3. Capture identifiers early: title, year, venue, DOI, arXiv id, project URL.
4. Separate "must-read" papers from "background only" papers.
5. Return a short evidence map instead of a loose list.

## Expected Outputs

- a ranked paper list
- a baseline list
- a source table with identifiers
- unresolved search gaps that require another pass

## Quality Rules

- prefer primary sources over blog summaries
- note publication year and venue whenever available
- call out uncertainty when a result is only weakly relevant
- do not claim a benchmark or baseline is standard without evidence
