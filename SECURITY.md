# Security Policy

The Leyton CognitX team takes the security of our software, and our users, seriously. This document explains how to report vulnerabilities in any repository under the [`cognitx-leyton`](https://github.com/cognitx-leyton) organization.

## Supported Versions

For each repository, security fixes are applied to the **latest released version** on `main`. Older versions are supported only on a best-effort basis. If a project publishes long-term support branches, that will be called out in its own `README.md`.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.**

Instead, report them privately through one of the following channels:

1. **GitHub Private Vulnerability Reporting** (preferred) — on the affected repository, click **Security → Report a vulnerability**. This creates a private advisory visible only to maintainers.
2. **Email** — send a report to [cognitx@leyton.com](mailto:cognitx@leyton.com) with the subject line `[SECURITY] <repo-name> — <short description>`.

Please include as much of the following as you can:

- The repository and version (commit SHA, tag, or package version) affected
- A description of the vulnerability and its potential impact
- Step-by-step instructions to reproduce the issue
- Any proof-of-concept code, logs, or screenshots
- Your assessment of severity (optional)
- Whether you'd like to be credited in the advisory, and under what name

You do not need to have a fix ready. A clear reproduction is the most valuable thing you can provide.

## What to Expect

- **Acknowledgement** within **2 business days** of receiving your report.
- **Initial triage** (confirming reproducibility and severity) within **5 business days**.
- **Regular updates** at least every 7 days while we investigate and fix the issue.
- **Coordinated disclosure** — we will work with you to agree on a disclosure timeline. Our default target is a fix within **90 days** of acknowledgement, sooner for critical issues.
- **Credit** — with your permission, we will credit you in the published security advisory once a fix is released.

## Scope

This policy covers all source code, build tooling, and published artifacts in the `cognitx-leyton` organization. It does **not** cover:

- Third-party dependencies — please report those upstream, and let us know if you believe we are affected
- Vulnerabilities in services operated by Leyton outside of this organization
- Social-engineering attacks against project maintainers or users

## Safe Harbor

We consider security research conducted in good faith under this policy to be:

- Authorized with respect to any applicable anti-hacking laws
- Exempt from restrictions in our terms of service that would conflict with this policy

We will not pursue or support legal action against researchers who follow this policy. If in doubt about whether a specific activity is covered, email us at [cognitx@leyton.com](mailto:cognitx@leyton.com) **before** you start — we're happy to clarify.

Thank you for helping keep Leyton CognitX and its users safe.
