# .github

Organization-wide GitHub configuration for Compound Foundation.

## policy-bot

`policy.yml` is the shared approval policy for [policy-bot](https://github.com/palantir/policy-bot), which runs from [policy-bot-deployer](https://github.com/Compound-Foundation/policy-bot-deployer). policy-bot reads this file from `main` on every evaluation and ignores `.policy.yml` files in individual repositories. A change here applies as soon as it merges, to every repository where the Compound Policy Bot GitHub App is installed.

`policy-tests/policy.yml` holds scenarios for `policy-bot test`. CI runs `policy-bot validate` and `policy-bot test` on every pull request. Add a scenario for each rule you add or change.
