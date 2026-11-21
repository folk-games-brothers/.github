# Folk Games Studio GitHub Defaults

This repository provides default community health files and reusable workflows for the `folk-games-brothers` organization.

## What is included

- `PULL_REQUEST_TEMPLATE.md`: default pull request template
- `CONTRIBUTING.md`: contribution and branch naming guide
- `.github/workflows/check-purpose-branch-creation-prs.yml`: reusable workflow for branch-purpose validation

## How other repositories use this

Repositories without their own community health files automatically inherit defaults from this repository.

Reusable workflows can be called from another repository:

```yaml
jobs:
  check-branch:
    uses: folk-games-brothers/.github/.github/workflows/check-purpose-branch-creation-prs.yml@master
```

## Custom actions

Custom composite actions should live in a dedicated `folk-games-brothers/actions` repository for clearer versioning and reuse.

## Default branch

`master`
