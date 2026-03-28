Checkpoint 1
    Commands Used:
        git add src/calculator.py
	    git commit -m “fix”
	    git add src/validator.py
	    git commit -m “update”

    I learned how to use the staging area to control what goes into each commit.

Checkpoint 2
    Commands Used:
	    git log –oneline
	    git revert 
        
    I learned how to undo a commit without deleting it from history using git revert.

Checkpoint 3
    Commands Used:
	    git switch main
	    git commit -m “Add is_positive helper function”
        git cherry-pick
        
    I learned how to move a commit from one branch to another using cherry-pick.

Checkpoint 4
    Commands Used:
	    git reflog
	    git branch -D experiment/rnair124
        git merge recovered/rnair124
        
    I learned how to recover lost work using git reflog.

Checkpoint 5
    Commands Used:
	    git remote add upstream
	    git merge –ff-only upstream/main
        git rebase main
        git push –force-with-lease
        
    I learned how to sync my branch with the upstream repository and rebase my changes.

Checkpoint 6
    Commands Used:
	    git log main..HEAD –oneline
	    git rebase -i main
        git push –force-with-lease
        
    I learned how to clean up commit history using interactive rebase.

Checkpoint 7
       
    I learned how to review teammates’ code and provide meaningful feedback to other peoples code through pull requests.