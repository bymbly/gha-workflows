# Github Actions Reusable Workflows

Reference reusable workflows from your repo like:

```yaml
name: Format Check

on:
  push:
    branches:
      - main
      - renovate/**
  pull_request:
  workflow_dispatch:

jobs:
  format:
    name: Format Check
    uses: bymbly/gha-workflows/.github/workflows/prettier-format-check.yaml@main
```

See individual workflows for optional and mandatory parameters.
