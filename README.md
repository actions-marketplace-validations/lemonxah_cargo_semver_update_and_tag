# Cargo Semver Update and Tag GitHub Action

GitHub Action that extracts Semver version from Cargo.toml file and updates the version before Tagging it.

## Inputs

- `GITHUB_TOKEN`

  **Required** GitHub Token needed for the commit and tag

## Example Usage

```yaml
jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Cargo Semver Update and Tag
        uses: lemonxah/cargo_semver_update_and_tag@v0.0.10
        with:
          GITHUB_TOKEN: ${{ github.token }}
```