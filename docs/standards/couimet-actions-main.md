# couimet GitHub Actions use @main

Source: rule `couimet-actions-main` in [couimet/github-actions README.md](https://github.com/couimet/github-actions/blob/main/README.md). That file is the only source. The block below stays equal to it.

```xml
<rule id="couimet-actions-main" priority="critical">
  <title>couimet/* GitHub Actions always use @main</title>
  <never>Pin a `couimet/*` GitHub Action to a commit SHA in workflows or composite action definitions</never>
  <do>Always reference `couimet/*` actions with `@main` to get the latest version</do>
  <rationale>The author wants these actions to auto-update across all repos</rationale>
</rule>
```
