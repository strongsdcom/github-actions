# Github Actions
This repo is for sharing different Github Actions workflows for corporate projects

## Release

Create releases with [`release-please-action`](https://github.com/googleapis/release-please-action).

Release-please configuration reference is [here](https://github.com/googleapis/release-please/blob/main/docs/manifest-releaser.md).

Example release-please configuration for an Elixir project:

```json
{
  "packages": {
    ".": {
      "release-type": "elixir",
      "bump-minor-pre-major": true,
      "bump-patch-for-minor-pre-major": false,
      "extra-files": [".deploy/Chart.yaml"]
    }
  }
}
```

Example workflow:

```yaml
name: Release

on:
  push:
    branches:
      - main

permissions:
  contents: write
  pull-requests: write

concurrency:
  group: ${{ github.workflow }}-${{ github.ref }}
  cancel-in-progress: true

jobs:
  release-please:
    uses: strongsdcom/github-actions/.github/workflows/release-please.yaml@v2
    with:
      config-file: .github/release-please/config.json
      manifest-file: .github/release-please/manifest.json
```

## Jira Release

Creates a Jira release and sets a fixed version for the found issues from github commits

Example of usage with custom GITHUB Token for Release Please can be found [here](examples/jira-release.yaml).

Example of usage in single file can be found [here](examples/release.yaml).

## Developoment

### Useful commands

```
awk '{$1=$1};1'                      # Removes leading and trailing spaces in multiline string
sed '/^$/d'                          # Removes empty rows in multiline string
sed 's/original-string/new-string/'  # Replace original text to new text in the string
sed 's/.*/prefix&suffix/'            # Replace each row to new prefixed and suffixed row in
                                     # multiline string
sed '$!N;s/\n/ /'                    # Replace multiline string to single line string
```
