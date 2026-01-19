Advanced Git Operations

This section covers advanced Git commands commonly used in real-world projects to manage history, releases, and complex workflows.

---

1. git rebase

"git rebase" reapplies commits from one branch onto another branch to create a clean, linear history.

Command

git rebase main

Example

You are working on "feature-login" and want the latest changes from "main":

git checkout feature-login
git rebase main

What happens:

- Feature commits are temporarily removed
- Latest "main" commits are applied
- Feature commits are replayed on top

📌 Best used before merging a feature branch
⚠️ Avoid rebasing shared branches

---

2. git cherry-pick

"git cherry-pick" applies a specific commit from one branch to another.

Command

git cherry-pick <commit-id>

Example

A critical bug fix exists on "dev" branch:

git checkout main
git cherry-pick abc123

📌 Useful for hotfixes and selective changes

---

3. git stash

"git stash" temporarily saves uncommitted changes and cleans the working directory.

Command

git stash

Example

You need to switch branches urgently:

git stash
git checkout main

📌 Best when work is not ready to commit

---

4. git stash pop

"git stash pop" restores the latest stashed changes and removes them from stash list.

Command

git stash pop

Example

Return to your work:

git checkout feature-login
git stash pop

📌 Conflicts may occur and must be resolved manually

---

5. git tag

"git tag" is used to mark specific commits, usually for releases.

---

Create a Lightweight Tag

git tag v1.0

Create an Annotated Tag (Recommended)

git tag -a v1.0 -m "Release version 1.0"

List Tags

git tag

Push Tags to Remote

git push origin v1.0

📌 Commonly used for release versions (v1.0, v2.0)

---

6. git merge vs git rebase

git merge

- Combines branches with a merge commit
- Preserves complete history
- Safe for shared branches

git checkout main
git merge feature-login

📌 Best for team collaboration and production branches

---

git rebase

- Rewrites commit history
- Creates linear history
- Cleaner commit logs

git checkout feature-login
git rebase main

📌 Best for local feature branches

---

7. When to Use What

Scenario| Recommended
Feature branch (local)| "git rebase"
Shared branch| "git merge"
Production fix| "git cherry-pick"
Work in progress| "git stash"
Release versioning| "git tag"

---

8. Summary

- "git rebase" → clean history
- "git merge" → safe collaboration
- "git cherry-pick" → selective commits
- "git stash" → temporary save
- "git tag" → release marking

These commands are essential for advanced Git workflows used in professional development and DevOps environments.
