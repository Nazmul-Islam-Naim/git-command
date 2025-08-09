## 1. Junior Developer Commands (Basic)
**Goal:** Work safely on their own branch.

```bash
git clone <repo-url>
git status
git add <file>         # stage one file
git add .              # stage all changes
git commit -m "Meaningful message"
git pull origin <branch>
git push origin <branch>
git checkout -b <branch-name>
git checkout <branch-name>
2. Intermediate Developer Commands (Intermediate)
Goal: Handle conflicts, history cleanup, and review PRs.

All Junior commands plus:

bash
Always show details

Copy
git log --oneline --graph --decorate
git merge <branch>
git rebase <branch>

# After fixing conflicts
git add <file>
git commit

# Undo commits
git reset --soft HEAD~1
git reset --hard HEAD~1

# Revert or apply commits
git revert <commit-hash>
git cherry-pick <commit-hash>
3. Senior Developer Commands (Advanced)
Goal: Manage repo health, recover lost work, and set workflows.

All Junior + Intermediate commands plus:

bash
Always show details

Copy
# Rewrite history
git rebase -i <commit-hash>

# Recover lost commits
git reflog

# Remove sensitive files
git filter-repo --path <file> --invert-paths

# Large file storage
git lfs install
git lfs track "*.psd"

# Submodules
git submodule add <repo-url> <path>
git submodule update --init --recursive

# Signed commits
git commit -S -m "Signed commit"

# Tags
git tag -a v1.0 -m "Release v1.0"
git push origin v1.0
"""
