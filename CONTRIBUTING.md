# Contributing to Leyton CognitX

Thank you for your interest in contributing! We welcome contributions from the community across all our open source projects.

## Getting Started

1. **Fork** the repository you want to contribute to
2. **Clone** your fork locally
3. **Create a branch** for your changes (`git checkout -b feat/your-feature`)
4. **Make your changes** and test them
5. **Commit** with a clear message describing what you changed and why
6. **Push** to your fork and open a **Pull Request**

## Branch model

Our repositories follow a three-branch protected model:

| Branch | Purpose |
| --- | --- |
| `main` | Production-ready code. Protected. All changes land here via PR. |
| `release` | Release-candidate stabilisation before tagging a version. Protected. |
| `hotfix` | Urgent fixes that need to skip the normal cycle. Protected. |

Day-to-day development happens on feature branches, typically cut from `main` (or from a long-lived `dev` branch when a repository uses one). Use descriptive prefixes:

- `feat/<short-description>` — new features
- `fix/<short-description>` — bug fixes
- `docs/<short-description>` — documentation
- `chore/<short-description>` — tooling, CI, refactors

All protected branches require at least one **Code Owner** approval before merging. See each repository's `CODEOWNERS` file for the list of reviewers. Force-pushes and branch deletions are disabled, and stale reviews are dismissed when new commits are pushed.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/) across the organization:

```
feat(parser): detect nestjs guards as decorator nodes
fix(loader): handle empty file nodes without crashing
docs(readme): add example query for cyclic dependencies
chore(ci): bump action versions
```

This keeps history readable and makes it easy to generate changelogs.

## Guidelines

- Keep PRs focused on a single change
- Follow the existing code style and conventions of the project
- Update documentation if your change affects usage
- Add tests where applicable
- Resolve conversations on your PR before merging

## Reporting Issues

- Use the **Issues** tab on the relevant repository
- Include steps to reproduce the problem
- Include your environment details (OS, language version, etc.)
- Check existing issues before opening a new one

## Reporting security issues

Please **do not** open a public issue for security vulnerabilities. Email [cognitx@leyton.com](mailto:cognitx@leyton.com) with a description and a reproduction, and we'll acknowledge within a few business days.

## Code of Conduct

Be respectful and constructive. We are committed to providing a welcoming and inclusive experience for everyone.

## Questions?

- Open a discussion or issue on the relevant repository
- Email us at [cognitx@leyton.com](mailto:cognitx@leyton.com)
- Visit [cognitx.leyton.com](https://cognitx.leyton.com/)

## License

By contributing, you agree that your contributions will be licensed under the same [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0) that covers the project.
