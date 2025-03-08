## Git Cheat Sheet - Concise

### Configuration (`git config`)

*   **`git config --list`**: Show all configs.
*   **`git config --list | grep <pattern>`**: Search configs.
*   **`git config --get <key>`**: Get config value.
*   **`git config --global <key> <value>`**: Set global config.
*   **`git config --local <key> <value>`**: Set local config.
*   **`git config --unset <key>`**: Unset config.
*   **`git config --remove-section <section>`**: Remove config section.
*   **`git config --global rerere.enabled true`**: Enable rerere (reuse recorded resolutions).

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
*   **`git log --grep="<pattern>"`**: Search commit messages.
*   **`git log --author="<name>"`**: Search by author.
*   **`git log --since="<date>"` --until="<date>"`**: Search by date range.
*   **`git log -- <file_path>`**: Show history for a file.
*   **`git reflog`**: Branch HEAD history (reflog).
*   **`git reflog -<n>`**: Last `<n>` reflog entries.
*   **`git cat-file -p <hash>`**: View Git object.
*   **`git bisect start`**: Start bisect session.
*   **`git bisect bad`**: Mark current commit as bad during bisect.
*   **`git bisect good <commit_hash>`**: Mark commit as good during bisect.
*   **`git bisect reset`**: End bisect session.
*   **`git revert <commit_hash>`**: Revert a commit (creates new commit).
*   **`git reset --soft <commit_hash>`**: Soft reset (keep staging & working dir).
*   **`git reset --mixed <commit_hash>`**: Mixed reset (default, keep working dir).
*   **`git reset --hard <commit_hash>`**: Hard reset (discard working dir changes - CAUTION!).

### Remotes

*   **`git remote add origin <url>`**: Add remote "origin".
*   **`git remote -v`**: List remotes.
*   **`git fetch`**: Download remote objects/refs.
*   **`git merge origin/<branch>`**: Merge remote branch.
*   **`git pull`**: Fetch & merge remote branch.
    *   Set upstream: `git branch --set-upstream-to=origin/<branch> <local_branch>`.
*   **`git push`**: Push local commits to remote.
    *   `git push origin <branch>`: Push specific branch.
    *   `git push origin --tags`: Push tags.
    *   `git push --force origin <branch>`: Force push (CAUTION!).
*   **`git branch -a`**: List all branches (local & remote).

### Stashing

*   **`git stash`**: Stash changes.
*   **`git stash list`**: List stashes.
*   **`git stash pop`**: Apply & remove latest stash.
*   **`git stash apply <stash_name>`**: Apply stash (keep in list).
*   **`git stash drop <stash_name>`**: Remove stash.

### Worktrees

*   **`git worktree add <path> <branch>`**: Create worktree for branch.
*   **`git worktree list`**: List worktrees.
*   **`git worktree remove <path>`**: Remove worktree.

### Tags

*   **`git tag -a <tag_name> -m "<message>"`**: Create annotated tag.
*   **`git tag <tag_name>`**: Create lightweight tag.
*   **`git tag`**: List tags.
*   **`git show <tag_name>`**: Show tag info.
*   **`git checkout tags/<tag_name>`**: Checkout tag (detached HEAD).

---

**Note:** Simplified cheat sheet. Use `git --help` for details. 
