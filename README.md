# Github Actions
This repo is for sharing different Github Actions workflows for corporate projects

## Release Please

https://github.com/google-github-actions/release-please-action

Example of usage can be found [here](examples/release-please.yaml).

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
