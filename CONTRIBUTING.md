# Contributing to AONE

Welcome!

Thank you for contributing to AONE.

Whether you're fixing a bug, implementing a feature, improving documentation, or reviewing code, your work helps build a reliable, scalable, and maintainable mobility platform.

This guide explains **how to contribute** to every repository within the AONE GitHub organization.

---

# Before You Start

Before writing any code, please read:

- Organization Profile
- README.md
- SECURITY.md
- CODEOWNERS

Every contributor is expected to understand the engineering workflow before contributing.

---

# Development Workflow

Every feature follows the same lifecycle.

```text
Idea
    ↓
Research
    ↓
Specification
    ↓
Planning
    ↓
GitHub Issue
    ↓
Feature Branch
    ↓
Development
    ↓
Testing
    ↓
Pull Request
    ↓
Review
    ↓
Merge
```

Never skip documentation or issue creation.

---

# Repository Responsibilities

Each repository owns one responsibility.

| Repository | Responsibility |
|------------|----------------|
| backend | APIs & business logic |
| customer-app | Customer mobile application |
| driver-app | Driver mobile application |
| fleet-app | Fleet owner mobile application |
| admin-panel | Internal administration portal |
| website | Public website |
| shared-sdk | Shared libraries |
| shared-types | Shared models |
| infrastructure | Cloud infrastructure |
| docs | Product & engineering documentation |
| architecture | System design |

Avoid duplicating responsibilities between repositories.

---

# Creating New Work

Before beginning development, ensure:

- Business requirement exists
- Feature specification exists
- GitHub Issue created
- Acceptance criteria defined
- Repository identified

Development should never begin without a tracked Issue.

---

# Branch Naming

Never commit directly to `main`.

Use descriptive branch names.

Examples

```
feature/customer-login

feature/live-tracking

fix/payment-timeout

refactor/auth-service

docs/api-standard

hotfix/payment-failure
```

Avoid

```
test

new

work

changes
```

---

# Commit Messages

AONE follows Conventional Commits.

Format

```text
type(scope): description
```

Examples

```text
feat(auth): implement otp login

fix(payment): retry failed payments

docs(prd): update booking flow

refactor(driver): simplify ride state machine
```

---

# Pull Requests

Every Pull Request should:

- Solve one logical problem
- Reference its GitHub Issue
- Update documentation when necessary
- Pass all CI checks
- Receive required approvals

Before requesting review verify:

- Feature complete
- Tests passing
- Documentation updated
- No merge conflicts
- Branch up to date

---

# Code Reviews

Reviews improve software quality.

Reviewers focus on:

- Correctness
- Maintainability
- Readability
- Security
- Performance
- Documentation

Reviews are collaborative—not personal.

---

# Testing

Before merging ensure:

- Unit tests pass
- Integration tests pass (where applicable)
- Manual verification completed
- Lint passes
- Type checking passes

Critical business functionality should always include automated tests.

---

# Documentation

Documentation is part of every feature.

Whenever implementation changes:

- APIs
- Architecture
- Business logic
- Database schema
- Configuration

update the corresponding documentation.

The `docs` repository is the single source of truth.

---

# Security

Never commit:

- API keys
- Secrets
- Passwords
- Tokens
- Credentials

Use:

- GitHub Secrets
- Environment Variables
- Secret Manager

Follow the guidelines in SECURITY.md.

---

# Need Help?

If you're blocked:

1. Explain the problem.
2. Describe what you've already tried.
3. Link the relevant Issue or Pull Request.
4. Ask for help early.

Communication is preferred over working in isolation.

---

# Engineering Handbook

This guide intentionally remains concise.

Detailed engineering standards are maintained in the `docs` repository.

Topics include:

- Engineering Constitution
- Git Workflow
- Repository Organization
- Issue Management
- Code Review Standards
- Coding Standards
- Testing Strategy
- Security
- Release Process
- Onboarding

Contributors are expected to follow those standards where applicable.

---

# Pull Request Checklist

Before requesting review:

- [ ] GitHub Issue linked
- [ ] Acceptance criteria satisfied
- [ ] Tests pass
- [ ] Documentation updated
- [ ] No secrets committed
- [ ] CI passes
- [ ] Branch is up to date
- [ ] Ready for review

---

# Guiding Principle

> Build software that is easy to understand, easy to maintain, and easy to scale.

When in doubt, choose the solution that improves long-term maintainability over short-term convenience.