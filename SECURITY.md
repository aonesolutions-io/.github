# Security Policy

Thank you for helping keep AONE secure.

Security is a shared responsibility across everyone contributing to the AONE GitHub organization. This document explains how to report vulnerabilities, our supported versions, and the security practices expected from all contributors.

---

# Scope

This policy applies to every repository within the AONE GitHub organization, including but not limited to:

- backend
- customer-app
- driver-app
- fleet-app
- admin-panel
- website
- shared-sdk
- shared-types
- infrastructure
- docs
- architecture
- .github

---

# Supported Versions

Only actively maintained branches receive security updates.

| Branch | Supported |
|---------|:---------:|
| main | ✅ |
| develop | ✅ |
| release/* | ✅ |
| feature/* | ❌ |
| archived branches | ❌ |

---

# Reporting a Vulnerability

**Please do not disclose security vulnerabilities publicly.**

Do NOT:

- Open a public GitHub Issue
- Discuss the vulnerability publicly
- Publish proof-of-concept exploits before a fix is available

Instead, report the issue privately to the AONE engineering team.

Include the following information whenever possible:

- Summary of the issue
- Repository affected
- Component or feature
- Steps to reproduce
- Expected behavior
- Actual behavior
- Potential impact
- Severity assessment
- Screenshots or logs (if applicable)
- Suggested mitigation (optional)

---

# Response Process

Our security response process follows these stages:

1. Report received
2. Initial acknowledgement
3. Risk assessment
4. Severity classification
5. Reproduction
6. Fix implementation
7. Internal testing
8. Release
9. Public disclosure (if appropriate)

---

# Severity Levels

## Critical

Examples:

- Remote code execution
- Authentication bypass
- Privilege escalation
- Production secrets exposure

Target response:
- Immediate

---

## High

Examples:

- Sensitive data exposure
- Authorization flaws
- Payment vulnerabilities
- Broken access control

Target response:
- As soon as possible

---

## Medium

Examples:

- Information disclosure
- Security misconfiguration
- Session weaknesses

Target response:
- Next planned security release

---

## Low

Examples:

- Missing security headers
- Minor hardening improvements
- Non-exploitable edge cases

Target response:
- Backlog / maintenance release

---

# Responsible Disclosure

We appreciate responsible disclosure.

Please:

- Give us reasonable time to investigate.
- Avoid accessing unnecessary user data.
- Avoid service disruption.
- Do not publicly disclose vulnerabilities before remediation.

---

# Security Best Practices

Contributors must never commit:

- API keys
- Passwords
- Secrets
- Private certificates
- Service account credentials
- Tokens
- `.env` files containing secrets

Always use:

- Environment Variables
- Secret Managers
- GitHub Secrets
- GCP Secret Manager

---

# Dependency Security

Repositories should:

- Keep dependencies updated
- Review dependency changes
- Resolve security advisories promptly
- Remove unused packages

---

# Code Review Requirements

Security-sensitive changes require additional review.

Examples include:

- Authentication
- Authorization
- Payments
- Encryption
- User permissions
- Infrastructure
- Deployment
- Secrets management

---

# Infrastructure Security

Infrastructure changes should:

- Follow least-privilege principles
- Be reviewed before deployment
- Be version controlled
- Avoid hardcoded credentials

---

# Documentation

Security-related architectural decisions should be documented in the `docs` repository.

Avoid duplicating documentation across repositories.

---

# Contact

Security reports should be sent through the organization's designated private communication channel.

Do not disclose vulnerabilities publicly until remediation has been completed.

---

# Thank You

We appreciate everyone who helps improve the security of AONE.

Responsible reporting helps protect our users, partners, and platform.