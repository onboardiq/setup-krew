# setup-krew
Github composite action to setup krew in linux OS

## Usage

This action currently supports Linux runners.

Add the following entry to your Github workflow YAML file:

```yaml
uses: onboardiq/setup-krew@main
with:
 krew-version: "latest" # optional. latest is default
```

Example:

```yaml
jobs:
  test-setup-krew:
    runs-on: ubuntu-latest
    name: Install Krew
    steps:
      - name: Install krew
        uses: onboardiq/setup-krew@main
      - name: Check install!
        run: kubectl-krew version
```
