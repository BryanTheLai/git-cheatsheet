## Git Cheat Sheet - Concise (Grouped by Usage Frequency)

### 🌟 Most Common (Daily) 🌟

*   **`git status`**:  Current repo status.
*   **`git add <file>` / `git add .`**: Stage changes for commit.
    *   `<file>`: Stage file.
    *   `.`: Stage all changes.
*   **`git commit -m "<message>"`**: Save staged changes locally.
*   **`git pull`**: Get remote changes & merge.
*   **`git push`**: Share local commits to remote.
*   **`git log --oneline`**: Compact commit history.
*   **`git branch`**: List local branches.
*   **`git checkout <branch_name>`**: Switch branch.
*   **`git checkout -b <new_branch_name>`**: Create & switch to new branch.

---

### Branching & Merging

*   **`git branch <new_branch_name>`**: Create new branch.
*   **`git merge <branch_name>`**: Merge branch into current.
*   **`git rebase <branch_name>`**: Rebase onto branch (linear history). *Careful on shared branches.*
*   **`git branch -D <branch_name>`**: Force delete branch (local). *Use with caution.*

---

### Remotes

*   **`git remote -v`**: List remote repos.
*   **`git remote add origin <repo_url>`**: Add remote named "origin".
*   **`git fetch`**: Download remote changes (no merge).
*   **`git branch -a`**: List all branches (local & remote).
*   **`git push origin <branch_name>`**: Push branch to remote.
*   **`git push origin --tags`**: Push tags to remote.

---

### History Inspection & Manipulation

*   **`git log`**: Detailed commit history.
*   **`git log --graph --oneline --decorate --all`**: Visual history graph.
*   **`git log --grep="<pattern>"`**: Search commit messages.
*   **`git log --author="<name>"`**: Filter by author.
*   **`git log -- <file_path>`**: History for file.
*   **`git reflog`**: Branch HEAD history (recovery).
*   **`git bisect start`**: Start bug hunt (binary search).
*   **`git bisect bad` / `git bisect good <commit_hash>` / `git bisect reset`**: Bisect commands.
*   **`git revert <commit_hash>`**: Undo commit (new commit). *Safe undo.*
*   **`git reset --soft <commit_hash>`**: Reset to commit (keep staged).
*   **`git reset --mixed <commit_hash>`**: Reset to commit (keep working dir). *Default reset.*
*   **`git reset --hard <commit_hash>`**: Reset to commit (discard changes). *Danger: Discards work!*

---

### Configuration & Setup

*   **`git init`**: Initialize new repo.
*   **`git config --list`**: Show config settings.
*   **`git config --global <key> <value>`**: Set global config.
*   **`git config --local <key> <value>`**: Set repo config.
*   **`git config --global rerere.enabled true`**: Enable reuse recorded resolutions.

---

### Stashing

*   **`git stash`**: Stash changes (clean work dir).
*   **`git stash list`**: List stashes.
*   **`git stash pop`**: Apply & remove latest stash.
*   **`git stash apply <stash_name>`**: Apply stash (keep in list).
*   **`git stash drop <stash_name>`**: Delete stash.

---

### Advanced & Less Frequent

*   **`git worktree add <path> <branch>`**: Create worktree for branch.
*   **`git worktree list`**: List worktrees.
*   **`git worktree remove <path>`**: Remove worktree.
*   **`git tag -a <tag_name> -m "<message>"`**: Create annotated tag.
*   **`git tag <tag_name>`**: Create lightweight tag.
*   **`git tag`**: List tags.
*   **`git show <tag_name>`**: Show tag details.
*   **`git checkout tags/<tag_name>`**: Checkout tag (detached HEAD).
*   **`git cat-file -p <hash>`**: View Git object content.
*   **`git push --force origin <branch_name>`**: Force push (override remote). *Danger: Rewrite history!*
*   **`git branch -D <branch_name>`**: Force delete branch (local). *Caution.*


---

**Note:**  `git --help <command>` for details. 
