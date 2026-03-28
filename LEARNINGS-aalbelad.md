# LEARNINGS-aalbelad.md

## CP1 – Staging vs Committing
Commands:
- git checkout -b feature/aalbelad starter/role-A
- pytest tests/
- git add src/validator.py tests/test_calculator.py
- git commit -m "fix"
- git add src/calculator.py
- git commit -m "update"

Reflection:
I learned how staging allows me to control exactly what goes into each commit. Separating the fix and update commits helped me understand how to create clear, meaningful commit history.

## CP2 – Reverting a Bad Commit
Commands:
- git log --oneline
- git revert <BAD_COMMIT_HASH>

Reflection:
I learned that git revert safely undoes a commit by creating a new commit instead of deleting history. This is important for collaboration because it keeps a full and transparent record of changes.

## CP3 – Moving a Commit with Cherry-Pick
Commands:
- git checkout main
- git add src/validator.py
- git commit -m "Add is_positive helper function"
- git log --oneline -1
- git reset --hard HEAD~1
- git checkout feature/aalbelad
- git cherry-pick <HASH>

Reflection:
I learned how to recover from committing on the wrong branch by using cherry-pick. This allows moving a specific change without rewriting the code manually.

## CP4 – Recovering Lost Work with Reflog
Commands:
- git checkout -b experiment/aalbelad
- git add src/calculator.py
- git commit -m "Experiment change"
- git checkout feature/aalbelad
- git branch -D experiment/aalbelad
- git reflog
- git checkout -b recovered/aalbelad <HASH>
- git checkout feature/aalbelad
- git merge recovered/aalbelad

Reflection:
I learned that even after deleting a branch, Git can recover lost commits using reflog. This shows that most mistakes in Git are reversible if you know the right tools.

## CP5 – Syncing with Upstream and Rebasing
Commands:
- git remote set-url upstream https://github.com/mdurrani808/git_project_1.git
- git fetch upstream
- git checkout main
- git reset --hard upstream/main
- git checkout feature/aalbelad
- git rebase main
- git push --force-with-lease origin feature/aalbelad

Reflection:
I learned how to synchronize my work with the latest changes from the original repository using rebase. This keeps the commit history clean and avoids unnecessary merge commits.

## CP6 – Cleaning Commit History
Commands:
- git log main..HEAD --oneline
- git rebase -i main
- git push --force-with-lease origin feature/aalbelad

Reflection:
I learned how to clean up commit history by rewriting commit messages using interactive rebase. This makes the project easier to review and improves code readability.

## CP7 – Pull Requests and Code Review
Commands:
- git push origin feature/aalbelad
- Open pull request (feature/aalbelad → main)
- Review teammate PR and request changes
- Respond to comments on my PR

Reflection:
I learned how to collaborate using pull requests by reviewing teammate code, requesting changes, and responding to feedback. This helped me understand how real-world team workflows operate in GitHub.