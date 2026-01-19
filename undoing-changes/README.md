# Undoing Changes in Git

Mistakes happen in development. Git provides powerful commands to **undo changes safely or forcefully** depending on the situation.

The most commonly used commands are:
- git reset
- git revert

---

## 1. git reset

git reset is used to **move the current branch (HEAD)** to a previous commit.

It directly modifies commit history and should be used **carefully**.

---

### Soft Reset

**What it does:**
- Removes the commit
- Keeps file changes in the **staging area**

git reset --soft HEAD~1

Example: You committed with a wrong message:

git commit -m "fix bug"

You want to rewrite the commit:

git reset --soft HEAD~1
git commit -m "Fix login validation bug"

📌 Use when you want to edit or squash commits.

###Hard Reset

**What it does:**

Removes the commit
Deletes all related file changes
Resets working directory and staging area

git reset --hard HEAD~1

Example: You made an experimental commit and want to remove it completely:

git reset --hard HEAD~1

⚠️ Warning: This action permanently deletes commits and changes.

📌 Use only for local and unshared work.

2. git revert

git revert safely undoes a commit by creating a new commit that reverses the changes.

Example: A bug was introduced in commit abc123:

git revert abc123

Git creates a new commit that cancels the changes made by abc123.

✔ Safe for shared branches
✔ Preserves full history
📌 Recommended for production and team environments.

###When to Use What

Use git reset → when working alone on local changes
Use git revert → when changes are already pushed
Prefer revert in collaborative projects

###Summary

git reset --soft → undo commit, keep changes
git reset --hard → undo commit and changes
git revert → safe undo with history preserved

Understanding these commands helps you fix mistakes without breaking your project history.
