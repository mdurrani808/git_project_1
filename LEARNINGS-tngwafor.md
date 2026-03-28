# LEARNINGS-tngwafor

## CP1
### Commands
```bash
git checkout starter/role-D
git checkout -b feature/tngwafor
git push -u origin feature/tngwafor
pytest tests/
git add tests/test_calculator.py
git commit -m "fix"
git add .gitignore
git commit -m "update"
git push origin feature/tngwafor

Reflection : 
I learned how to use the staging area to separate unrelated changes into different commits. This matters because clean commits make code review and debugging much easier.

Checkpoint 2
git log --oneline
git revert 6ca467b
pytest tests/
git push origin feature/tngwafor

Reflection : 
I learned how to undo a bad commit with git revert without deleting history. This matters because it preserves a clear project history while safely reversing unwanted changes.

Checkpoint 3
git checkout main
git add src/validator.py
git commit -m "Add is_positive helper function"
git log --oneline -1
git reset --hard HEAD~1
git checkout feature/tngwafor
git cherry-pick 8611771
git add src/validator.py
git cherry-pick --continue
pytest tests/
git push origin feature/tngwafor

Reflection :
I learned how to move work from the wrong branch to the correct one using git cherry-pick. This matters because mistakes happen, and knowing how to recover cleanly helps keep branches organized.


Checkpoint 4 : 
git checkout -b experiment/tngwafor
git add src/validator.py
git commit -m "Add experimental comment"
git checkout feature/tngwafor
git branch -D experiment/tngwafor
git reflog
git checkout -b recovered/tngwafor <lost-commit-hash>
git checkout feature/tngwafor
git merge recovered/tngwafor
pytest tests/
git push origin feature/tngwafor

Reflection :
I learned that git reflog can recover commits even after a branch is deleted. This matters because it provides a safety net when work seems lost.

Checkpoint 5 :
git fetch upstream
git checkout main
git reset --hard upstream/main
git checkout feature/tngwafor
git rebase main
pytest tests/
git push --force-with-lease origin feature/tngwafor


Reflection : 
I learned how to sync my branch with the latest upstream changes using fetch, reset, and rebase. This matters because it keeps my work up to date and reduces messy merge history.


Checkpoint 6 : 
git log main..HEAD --oneline
git rebase -i main
pytest tests/
git push --force-with-lease origin feature/tngwafor


Reflection :
I learned how to clean up commit history with interactive rebase by rewording and organizing commits. This matters because a clean history makes the development process easier to understand and review.


