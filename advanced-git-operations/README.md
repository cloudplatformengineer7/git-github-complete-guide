Advanced Git Operations

This section covers advanced Git commands commonly used in real-world projects to manage history, releases, and complex workflows.

git rebase

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
