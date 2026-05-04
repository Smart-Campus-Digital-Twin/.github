# 🤝 Contributing Guidelines & Workflow

> **Please read this entire document before making any contribution.**
> Following this workflow keeps the project clean, collaborative, and moving fast for everyone.

---

## 📋 Table of Contents

- [Getting Started](#getting-started)
- [Required Contribution Workflow](#required-contribution-workflow)
- [Branch Naming Conventions](#branch-naming-conventions)
- [Commit Message Standards](#commit-message-standards)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Code & Quality Standards](#code--quality-standards)
- [What NOT to Do](#what-not-to-do)
- [Communication](#communication)
- [Need Help?](#need-help)

---

## 🚀 Getting Started

1. **Fork** the repository (if you're an external contributor) or **clone** it directly (if you're a team member).
2. Read this document **fully** before writing any code.
3. Check the [Issues](../../issues) tab to find something to work on, or open a new issue describing your proposed change.

---

## ✅ Required Contribution Workflow

Follow these steps **in order** before writing a single line of code:

### 1. 🔍 Open or Find an Issue

- Check existing issues to avoid duplicate work.
- If no issue exists, **open one first** — describe the bug, feature, or improvement clearly.
- Use a descriptive title and provide as much context as possible.

### 2. 🙋 Assign Yourself

- You **do not need to wait for a maintainer to assign you.**
- Simply **assign yourself** to the issue and leave a comment like:
  > _"I'm working on this — will open a PR soon."_
- This prevents two people from working on the same thing at the same time.

### 3. 🌿 Create a Branch

- Branch off from `main` (or the designated base branch).
- Follow the [branch naming conventions](#branch-naming-conventions) below.
- Never work directly on `main` or any protected branch.

```bash
# Example
git checkout main
git pull origin main
git checkout -b feat/your-feature-name
```

### 4. 💻 Do Your Work

- Implement the change with care.
- Write or update **tests** for your changes.
- Update **documentation** if applicable.
- Keep your changes focused — one issue, one PR.

### 5. 🔁 Open a Pull Request

- Link your PR to the issue using GitHub keywords (e.g., `Closes #42`).
- Fill out the PR template completely.
- Request **at least one reviewer** before marking it ready.
- Keep the PR small and reviewable — avoid bundling unrelated changes.

### 6. ✅ Await Review & Merge

- A maintainer or peer will review your PR.
- **Resolve all review comments** before requesting a re-review.
- Do not merge your own PR unless explicitly permitted.
- Once approved, a maintainer will merge it.

---

## 🌿 Branch Naming Conventions

Use the following prefixes to keep branches organized:

| Type | Pattern | Example |
|------|---------|---------|
| New feature | `feat/short-description` | `feat/user-auth` |
| Bug fix | `fix/short-description` | `fix/login-crash` |
| Documentation | `docs/short-description` | `docs/update-readme` |
| Refactor | `refactor/short-description` | `refactor/api-client` |
| Testing | `test/short-description` | `test/auth-unit-tests` |
| Hotfix | `hotfix/short-description` | `hotfix/null-pointer` |
| Chore | `chore/short-description` | `chore/update-deps` |

> Keep branch names **lowercase**, use **hyphens** (not underscores or spaces), and keep them **short but descriptive**.

---

## 💬 Commit Message Standards

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short description>

[optional body]

[optional footer — e.g., Closes #42]
```

### Commit Types

| Type | When to use |
|------|------------|
| `feat` | A new feature |
| `fix` | A bug fix |
| `docs` | Documentation changes only |
| `style` | Formatting, missing semicolons, etc. (no logic change) |
| `refactor` | Code restructuring without feature or bug change |
| `test` | Adding or updating tests |
| `chore` | Build process, dependency updates, tooling |
| `perf` | Performance improvements |

### Examples

```bash
feat(auth): add Google OAuth login
fix(api): handle null response from user endpoint
docs(contributing): update branch naming section
chore(deps): upgrade axios to v1.6.0
```

> ✅ Keep the subject line under **72 characters**.
> ✅ Use the **imperative mood** — "add feature" not "added feature".
> ✅ Reference the issue in the footer — `Closes #42`.

---

## 📝 Pull Request Guidelines

When opening a PR, make sure to:

- [ ] Use a clear, descriptive PR title following commit conventions
- [ ] Link the related issue (`Closes #<issue-number>`)
- [ ] Describe **what** changed and **why**
- [ ] List any **breaking changes** if applicable
- [ ] Confirm tests pass locally
- [ ] Request at least **one reviewer**
- [ ] Resolve **all review comments** before re-requesting review
- [ ] Do not merge your own PR

**PR Title Examples:**
```
feat(dashboard): add weekly activity chart
fix(notifications): prevent duplicate push alerts
```

---

## 🛠️ Code & Quality Standards

- Follow the existing **code style** of the project (linting rules apply).
- Write **clean, readable code** — prefer clarity over cleverness.
- Add **comments** for complex logic.
- Write or update **unit/integration tests** for every meaningful change.
- Ensure all existing tests pass before opening a PR.
- Avoid committing:
  - `.env` files or secrets
  - `node_modules/`, build artifacts, or IDE config files
  - Commented-out dead code

---

## 🚫 What NOT to Do

| ❌ Don't | ✅ Do Instead |
|---------|-------------|
| Open a PR without a linked issue | File or find an issue first |
| Push code directly to `main` or protected branches | Always work on a feature branch and go through a PR |
| Work on an issue someone else is already assigned to | Check assignees, find an unassigned issue |
| Skip reading this document | Read it fully before starting |
| Submit a PR with unrelated changes bundled together | One issue → one PR |
| Push `.env` files, secrets, or credentials | Add sensitive files to `.gitignore` |
| Go silent on an in-progress issue for many days | Post an update or unassign yourself |
| Request a re-review without resolving comments | Resolve all comments first |

> ⛔ **Direct pushes to `main` or any protected branch are strictly prohibited.**
> Every change must go through a Pull Request and pass code review.

---

## 💬 Communication

**Keep the team in the loop at all times.**

- 📱 **WhatsApp Group** — For quick updates, blockers, and informal discussion.
- 💬 **GitHub Discussions** — For broader decisions, proposals, and announcements.
- 🐛 **GitHub Issue Threads** — For all task-specific technical discussion (keep it here so it's traceable).

### Guidelines

- Ask questions **early** — don't wait until you're completely blocked.
- If you **can't complete** an assigned issue, comment on it and unassign yourself so someone else can pick it up.
- Post a quick update in the issue if your work is taking longer than expected.
- Silence on an in-progress task for several days may result in it being reassigned.

---

## ❓ Need Help?

- Browse the [existing issues](../../issues) and [discussions](../../discussions).
- Drop a message in the **WhatsApp group** for quick help.
- Comment directly on the relevant GitHub issue.
- Tag a maintainer in a discussion if you're stuck on something critical.

---

> ⚠️ **Failure to follow this workflow may result in PRs being closed without review.**
>
> We appreciate every single contribution — let's keep the process smooth, respectful, and productive for everyone. 🙌
