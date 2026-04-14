# AgentWorld Skills

AgentWorld supports a repository-local skill marketplace under `skills/`.

Each skill is a reusable package of execution guidance that can be loaded by one operator node without forcing the same behavior onto every other node in the graph.

## Structure

Each skill usually lives in its own folder:

```text
skills/
└── skill-name/
    ├── SKILL.md
    ├── references/
    ├── scripts/
    └── assets/
```

Only `SKILL.md` is required. The other folders are optional.

## Included Skills

| Skill | Purpose |
| --- | --- |
| `research-paper-search` | paper discovery, identifier collection, source triage |
| `literature-synthesis` | theme extraction, contradiction mapping, gap analysis |
| `citation-audit` | bibliography validation, metadata checks, citation hygiene |
| `experiment-planning` | executable research plans, deliverables, validation gates |
| `result-audit` | output review, unsupported claim detection, evidence checks |

## Usage

Attach skills directly to a graph node:

```python
graph.add_node(
    "plan",
    operator="planner",
    objective="Search the literature and frame the study",
    skills=["research-paper-search", "literature-synthesis"],
)
```

The runtime injects the selected skill names into the operator request, so the operator can build prompts and execution context for that specific node.

## Notes

- Skills are public project assets and should stay in English
- Skills should be specific enough to be reusable, but not so narrow that they only fit one task
- If a skill needs code or references, keep them inside the skill folder
- Private working notes belong in ignored local files, not in `skills/`
