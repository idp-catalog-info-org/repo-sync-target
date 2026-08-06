# Git Sync Target Repository

This repository is the **dedicated sync target** for Harness IDP Catalog Info YAML integration tests.

## Usage

- **TC-015** (Sync to Source Repo): uses the source repos as sync targets
- **TC-016** (Dedicated Repo): point `sync_repo` to this repo + `sync_branch` = `main`

After git sync runs, the IDP will write catalog YAML files under `.harness/idp/` in this repo.

## Expected Structure After Sync
```
.harness/
  idp/
    <entity-namespace>/<entity-kind>/<entity-name>/catalog-info.yaml
```
