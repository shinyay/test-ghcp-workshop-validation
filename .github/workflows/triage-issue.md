---
name: "Triage Issue (validation)"
description: "Validate gh aw safe-outputs add-labels and add-comment on a real issue"
on:
  issues:
    types: [opened]
permissions:
  contents: read
safe-outputs:
  add-labels:
    allowed: [bug, feature, question, docs]
  add-comment:
    max: 1
---

## Triage Issue

When a new issue is opened, classify it into exactly one of these categories
based on the issue body and title:

- **bug** — something is broken or behaves incorrectly
- **feature** — request for new functionality
- **question** — asking how to do something
- **docs** — documentation improvement

Then:

1. Add the chosen category as a label via safe-outputs.
2. Post one short greeting comment that:
   - confirms the chosen category
   - if it is a bug, asks for any obvious missing reproduction info (browser, OS, steps)

Do not modify the issue title or body.
