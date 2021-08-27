# auto-update-flake
GitHub Action to automatically update flake inputs if they pass CI

## Usage

Create .github/workflows/update.yml in your repo with the following contents:

```
name: "Update Flake"
on:
  schedule: "*/5 * * * *"
jobs:
  update-flake:
    runs-on: ubuntu-latest
    steps:
    - uses: matthewbauer/auto-update-flake@v0.0.1
```
