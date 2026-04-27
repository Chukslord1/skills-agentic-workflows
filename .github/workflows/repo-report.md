---
on:
  workflow_dispatch:

permissions:
  contents: read

tools:
  github:

safe-outputs:
  create-issue:
    title-prefix: "[repo-report] "
    labels: ["report"]
---

# Repository Report

Generate a report about this repository.

Include:
- Recent commits
- Open pull requests