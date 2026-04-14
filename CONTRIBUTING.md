# Contributing to Leyton CognitX

Thank you for your interest in contributing! We welcome contributions from the community across all our open source projects, and we want every contributor to feel welcome, included, and supported.

This guide applies to every repository under the [`cognitx-leyton`](https://github.com/cognitx-leyton) organization. Individual repositories may add their own setup or testing instructions in their `README.md` — always check there first for language- and stack-specific details.

## Quick Links

- [Code of Conduct](./CODE_OF_CONDUCT.md)
- [Security Policy](./SECURITY.md)
- [Open source portal](https://cognitx.leyton.com/)
- [All repositories](https://github.com/cognitx-leyton)
- Contact: [cognitx@leyton.com](mailto:cognitx@leyton.com)

## 1. Ways to Contribute

You don't need to write code to make a difference. Useful contributions include:

- Reporting bugs and edge cases
- Suggesting features and improvements
- Improving documentation, examples, and READMEs
- Reviewing open pull requests
- Helping other users in issues and discussions
- Writing or improving tests

## 2. Getting Started

1. **Find** a repository you want to contribute to under [cognitx-leyton](https://github.com/cognitx-leyton)
2. **Read** its `README.md` for setup, build, and test instructions — each project may use a different language and toolchain (Laravel/PHP, TypeScript/Node, Vue, Python, etc.)
3. **Fork** the repository
4. **Clone** your fork locally
5. **Create a branch** from `dev` (or `main` if the repo has no `dev`) — see the branch model below
6. **Make your changes** and test them locally
7. **Commit** with a signed, conventional message (see sections 4 and 5)
8. **Push** to your fork and open a **Pull Request** against the repository's base branch

### Good first issues

New to the project? Filter issues by the [`good first issue`](https://github.com/search?q=org%3Acognitx-leyton+label%3A%22good+first+issue%22+state%3Aopen&type=issues) label across the organization to find a friendly starting point.

## 3. Branch Model

Our repositories follow a protected branch model:

| Branch | Purpose | Protected |
| --- | --- | --- |
| `main` | Production-ready code. All changes land here via PR. | Yes |
| `release` | Release-candidate stabilisation before tagging a version. | Yes |
| `hotfix` | Urgent fixes that need to skip the normal cycle. | Yes |
| `dev` | Integration branch where day-to-day work lands first (when the repo uses one). | No |

Feature branches are typically cut from `dev` (or from `main` when a repo has no `dev`). Use descriptive prefixes:

- `feat/<short-description>` — new features
- `fix/<short-description>` — bug fixes
- `docs/<short-description>` — documentation
- `chore/<short-description>` — tooling, CI, refactors
- `test/<short-description>` — tests only

All protected branches require at least one **Code Owner** approval before merging. See each repository's `CODEOWNERS` file for the list of reviewers. Force-pushes and branch deletions are disabled, and stale reviews are dismissed when new commits are pushed.

## 4. Commit Messages

We use [Conventional Commits](https://www.conventionalcommits.org/) across the organization. This keeps history readable and makes it easy to generate changelogs.

```
feat(parser): detect nestjs guards as decorator nodes
fix(loader): handle empty file nodes without crashing
docs(readme): add example query for cyclic dependencies
chore(ci): bump action versions
test(export): cover chunked queue failure path
```

Scope (the part in parentheses) is optional but encouraged — use the module, package, or area most affected.

## 5. Developer Certificate of Origin (DCO)

All contributions must be signed-off to indicate agreement with the [Developer Certificate of Origin](https://developercertificate.org/). Sign off each commit with the `-s` flag:

```shell
git commit -s -m "feat(api): add pagination to list endpoint"
```

You can set up a convenient alias:

```shell
git config alias.cos "commit -s"
# then use: git cos -m "..."
```

The sign-off appends a `Signed-off-by: Your Name <your@email>` trailer to the commit message. CI will reject unsigned commits on protected branches.

## 6. Pull Requests

When opening a PR:

- **Keep it focused** — one logical change per PR. Split unrelated work.
- **Target the right base** — `dev` if it exists, otherwise `main`.
- **Fill in the PR template** — what, why, how you tested, linked issues.
- **Include tests** — new features and bug fixes should come with tests that fail without the change.
- **Update documentation** — if the change affects usage, public APIs, or configuration.
- **Follow the existing style** — match the conventions and tooling already in the repo (formatters, linters, type checkers).
- **Resolve conversations** — address or explicitly acknowledge every review comment before requesting re-review.
- **Keep CI green** — don't merge with failing checks.

PRs are reviewed by Code Owners. We aim to give first feedback within 2 business days.

## 7. Reporting Issues

Use the **Issues** tab on the relevant repository. Please include:

- A clear title and description
- Steps to reproduce
- Expected vs actual behaviour
- Environment details (OS, language version, relevant package versions)
- A minimal reproduction (code snippet, failing test, or small repo) when possible

Search existing issues before opening a new one to avoid duplicates.

### Issue labels

We use a common set of labels across repositories to help you navigate:

- `good first issue` — perfect for newcomers
- `help wanted` — extra attention or community help welcome
- `bug` — something isn't working as expected
- `enhancement` — new feature or improvement
- `documentation` — docs-only changes
- `question` — request for clarification or information
- `wontfix` — will not be worked on (with explanation)

## 8. Reporting Security Issues

**Please do not open a public issue for security vulnerabilities.** See our [Security Policy](./SECURITY.md) for how to report privately and what to expect in return.

## 9. Code of Conduct

All contributors are expected to follow our [Code of Conduct](./CODE_OF_CONDUCT.md). Be respectful, constructive, and patient — everyone was new once.

## 10. Getting Help

- Open a **Discussion** or **Issue** on the relevant repository
- Email us at [cognitx@leyton.com](mailto:cognitx@leyton.com) for sensitive or business inquiries
- Visit [cognitx.leyton.com](https://cognitx.leyton.com/)

We aim to respond to communications within 2 business days.

## 11. License

By contributing, you agree that your contributions will be licensed under the same [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0) that covers the project, unless the repository explicitly states otherwise in its `LICENSE` file.

---

Thank you for helping make Leyton CognitX better.
