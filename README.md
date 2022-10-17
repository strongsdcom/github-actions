# reusable-workflow
This repo is for sharing different Github Actions workflows for corporate projects

## Jira Release

In addition to the normal release, creates a Jira release and sets a fixed version for the found issues from github commits

Example of usage:

```yaml
jobs:
  release:
    uses: bit4coinBV/reusable-workflow/.github/workflows/release.yaml@main
    secrets:
      github-token: ${{ secrets.GITHUB_TOKEN }}
      jira-email: ${{ secrets.JIRA_EMAIL }}
      jira-token: ${{ secrets.JIRA_TOKEN }}
    with:
      release-type: 'elixir'
      extra-files: |
        .deploy/Chart.yaml
        apps/b4c_trade/mix.exs
     jira-project-key: 'SRE'
     jira-sub-domain: 'hyphe'
```     
