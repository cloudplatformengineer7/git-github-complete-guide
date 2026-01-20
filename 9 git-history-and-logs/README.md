Git History and Logs

Git provides powerful commands to inspect commit history, analyze changes, and understand project evolution.
These commands are essential for debugging, auditing, and reviewing code.

---

1. Git Log Commands

View Complete Commit History

git log

Displays detailed information such as commit hash, author, date, and message.

---

Compact One-Line History

git log --oneline

Shows each commit in a single line for quick review.

---

Custom One-Line Format

git log --pretty=oneline

Displays full commit hashes with commit messages in one line.

---

View Last N Commits

git log -3

Shows the most recent 3 commits.

---

Visualize Branching and Merging

git log --graph --oneline --all

Displays commit history as a graph across all branches.

---

2. Inspecting a Specific Commit

Show Details of a Commit

git show <commit-id>

Displays:

- Commit metadata
- Code changes
- Diff information

---

Show Only File Names Changed in a Commit

git show <commit-id> --name-only

Useful for quickly identifying affected files.

---

3. File-Specific History

Track History of a File (Including Renames)

git log --follow --all <filename>

Shows the complete history of a file, even if it was renamed or moved.

---

4. Common Use Cases

- Debugging – find when a bug was introduced
- Auditing changes – track who changed what and why
- Understanding history – analyze project and file evolution

---

5. Summary

- "git log" → explore commit history
- "git show" → inspect a specific commit
- "--graph" → visualize branches and merges
- "--follow" → track file history across renames

These commands help you understand, audit, and debug your Git repositories effectively.
