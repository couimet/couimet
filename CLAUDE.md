# couimet

This repository serves two purposes. It renders the GitHub profile README, and it holds the canonical cross-project standards for repositories maintained by `couimet`.

## Standards

`docs/standards/` holds the canonical cross-project policy, and `docs/standards/README.md` is the index. Change a standard through a pull request in this repository, and describe the affected repository types and the migration impact in that pull request.

## GitHub Actions references

Rules that govern how a workflow or a composite action references GitHub Actions. The rules are checked on every response; violations are unacceptable.

### couimet-actions-main: couimet GitHub Actions always use `@main`

<rule id="couimet-actions-main" priority="critical">
  <title>couimet/* GitHub Actions always use @main</title>
  <never>Pin a `couimet/*` GitHub Action to a commit SHA in workflows or composite action definitions</never>
  <do>Always reference `couimet/*` actions with `@main` to get the latest version</do>
  <rationale>The author wants these actions to auto-update across all repos</rationale>
</rule>

The canonical copy of this rule lives at `docs/standards/couimet-actions-main.md`, and the block above is identical to it.

## Docs CI

The CI workflow at `.github/workflows/ci.yml` lints and formats Markdown through `couimet/github-actions/markdownlint@main` and `couimet/github-actions/prettier@main`, and it checks links through `couimet/github-actions/validate-links@main`.
