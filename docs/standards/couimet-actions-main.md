# couimet GitHub Actions use @main

Source: the rule comes from [couimet/github-actions](https://github.com/couimet/github-actions). This file is the canonical copy. Copy the block below into a repository's CLAUDE.md file.

```xml
<rule id="couimet-actions-main" priority="critical">
  <title>couimet/* GitHub Actions always use @main</title>
  <never>Pin a `couimet/*` GitHub Action to a commit SHA in workflows or composite action definitions</never>
  <do>Always reference `couimet/*` actions with `@main` to get the latest version</do>
  <rationale>The author wants these actions to auto-update across all repos</rationale>
</rule>
```
