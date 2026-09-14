# Standards

Canonical cross-project standards for repositories maintained by `couimet`. They live in `couimet/couimet` and change through pull requests.

## Purpose

A standard records a convention that more than one repository must follow. This repository holds the canonical copy, so a repository that adopts a standard links to one source instead of keeping a second copy that drifts.

## Scope

A convention belongs here when it applies to more than one repository maintained by `couimet`. A convention that governs one repository alone stays in that repository.

## Adoption

A repository adopts a standard in one of two ways. It links to the standard when a reader can follow the link. It copies a rule block into its own instruction file when the tooling must read the rule locally, such as a `CLAUDE.md` file that Claude Code loads from the repository root.

## Index

| Standard                           | Path                                                                | Source                 | Status    |
| ---------------------------------- | ------------------------------------------------------------------- | ---------------------- | --------- |
| README Badge Policy                | [docs/standards/readme-badges.md](./readme-badges.md)               | couimet/idea-garden    | Published |
| couimet GitHub Actions use `@main` | [docs/standards/couimet-actions-main.md](./couimet-actions-main.md) | couimet/github-actions | Published |

## Change Process

Change a standard through a pull request in `couimet/couimet`. Every change describes the affected repository types and the migration impact. Small clarifications and typo fixes follow the same process, so every revision stays reviewable and version-controlled.

A standard that copies a block from another repository stays equal to that source by this process alone. No automated check compares the two copies. Update both copies in the same change.
