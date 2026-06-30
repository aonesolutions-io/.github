# AONE Organization Configuration

This repository contains organization-wide standards, templates, and engineering guidance for AONE.

Every repository in the organization can inherit behavior from this repository through GitHub's special `.github` conventions.

## Contents

- `profile/README.md` - the public organization page shown on GitHub
- `CONTRIBUTING.md` - contribution workflow and expectations
- `SECURITY.md` - vulnerability reporting guidance
- `CODEOWNERS` - default reviewers and ownership rules
- `PULL_REQUEST_TEMPLATE.md` - pull request checklist
- `.github/ISSUE_TEMPLATE/` - issue forms for bugs, features, docs, and research

## Reference Repositories

- docs - source of truth for business, product, engineering, and operational documentation
- architecture - system design and architecture guidance

## Why this repository exists

- Keep organization-wide collaboration rules in one place
- Avoid duplicating contribution guidance across projects
- Provide consistent issue and pull request workflows
- Support a clear separation between public organization branding and internal engineering documentation

## Notes

- Keep this repository private
- Use `main` as the default branch
- Protect `main` with pull request reviews and status checks
