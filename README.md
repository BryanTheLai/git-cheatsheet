## Git Cheat Sheet - Concise

### Configuration (`git config`)

*   **`git config --list`**: Show all configs.
*   **`git config --list | grep <pattern>`**: Search configs.
*   **`git config --get <key>`**: Get config value.
*   **`git config --global <key> <value>`**: Set global config.
*   **`git config --local <key> <value>`**: Set local config.
*   **`git config --unset <key>`**: Unset config.
*   **`git config --remove-section <section>`**: Remove config section.

### Basic Workflow

*   **`git init`**: New repo.
*   **`git status`**: Show status.
*   **`git add <file>` / `git add .`**: Stage changes.
    *   `<file>`: Stage file.
    *   `.`: Stage all.
*   **`git commit -m "<message>"`**: Commit changes.

### Branching & Merging

*   **`git branch`**: List branches.
*   **`git branch <name>`**: Create branch.
*   **`git checkout <name>`**: Switch branch.
*   **`git checkout -b <name>`**: Create & switch branch.
*   **`git merge <branch>`**: Merge branch.
*   **`git branch -D <name>`**: Force delete branch.
*   **`git rebase <branch>`**: Rebase branch.

### History

*   **`git log`**: Commit history.
*   **`git log --oneline`**: Compact history.
*   **`git log --graph --oneline --decorate --all`**: Visual history graph.
*   **`git reflog`**: Branch HEAD history (reflog).
*   **`git reflog -<n>`**: Last `<n>` reflog entries.
*   **`git cat-file -p <hash>`**: View Git object.

### Remotes

*   **`git remote add origin <url>`**: Add remote "origin".
*   **`git remote -v`**: List remotes.
*   **`git fetch`**: Download remote objects/refs.
*   **`git merge origin/<branch>`**: Merge remote branch.
*   **`git pull`**: Fetch & merge remote branch.
    *   Set upstream: `git branch --set-upstream-to=origin/<branch> <local_branch>`.
*   **`git branch -a`**: List all branches (local & remote).

---

**Note:** Simplified cheat sheet. Use `git --help` for details.
