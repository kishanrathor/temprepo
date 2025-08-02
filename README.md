
Git Commands Cheat Sheet
1. Git Configuration

```bash
git --version
```
- Check Git version installed.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
- Set global Git username and email.

---
2. Git Repository Setup
```bash
git init
```
- Initialize a new local Git repository.
```bash
git clone <repository-url>
```
- Clone an existing repository from GitHub.
---
3. File Operations
```bash
git status
```
- Check the status of working directory and staging area.
```bash
git add filename
git add .
```
- Stage file(s) for commit.
```bash
git reset filename
```
- Unstage a file.

```bash
git rm filename
```
- Delete a file from working directory and stage the deletion.

---
 4. Commit Changes

```bash
git commit -m "Your message"
```
- Commit staged changes with a message.

```bash
git commit -a -m "Your message"
```
- Automatically stage and commit tracked files.

---
5. View History

```bash
git log
```
- Show commit history.

```bash
git log --oneline
```
- Show condensed commit history.

```bash
git show <commit-id>
```
- Show details of a specific commit.

---
6. Branching

```bash
git branch
```
- List branches.

```bash
git branch <branch-name>
```
- Create a new branch.

```bash
git checkout <branch-name>
```
- Switch to another branch.

```bash
git checkout -b <branch-name>
```
- Create and switch to a new branch.

```bash
git branch -d <branch-name>
```
- Delete a branch.

---

## 🔁 7. Merging

```bash
git merge <branch-name>
```
- Merge a branch into current branch.

8. Push & Pull

```bash
git remote add origin <url>
```
- Add a remote repository.

```bash
git push -u origin main
```
- Push code to remote main branch.

```bash
git pull
```
- Fetch and merge changes from remote.

```bash
git fetch
```
- Fetch updates from remote (no merge).

---
 9. Undoing Changes

```bash
git checkout -- <file>
```
- Discard local changes to a file.

```bash
git reset --hard
```
- Reset all changes to last commit.

```bash
git revert <commit-id>
```
- Revert a specific commit.

```bash
git clean -fd
```
- Delete untracked files and directories.

---
 10. Stash Changes

```bash
git stash
```
- Save uncommitted changes.

```bash
git stash apply
```
- Re-apply saved changes.

```bash
git stash pop
```
- Re-apply and remove stash.

---
11. Tags

```bash
git tag
```
- List all tags.

```bash
git tag <tagname>
```
- Create a new tag.

```bash
git push origin <tagname>
```
- Push tag to remote.

---

---

12. Basic Cherry-Pick

```bash
git cherry-pick <commit-hash>
