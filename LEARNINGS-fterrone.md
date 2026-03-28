Checkpoint 1
- git switch -c feature/fterrone 
- git add .
- git commit -m "fix"             
- git add .
- git commit -m "update"
- git push origin feature/fterrone 

During this checkpoint, I learned how to add files to the staging area, commit them, and push them.

Checkpoint 2
- git log --oneline
- git revert b19f233

This checkpoint taught me how to undo commits without deleting them from the history using revert.

Checkpoint 3
- Git switch main
- git add .
- git commit -m "Add is_positive helper function"
- git log --oneline                              
- git reset --hard HEAD~1
- git switch  feature/fterrone                         
- git cherry-pick ed58ac4
- git add .
- git cherry-pick --continue
- git push origin feature/fterrone   

This checkpoint taught me how to delete a branch and recover the comment. It also taught me how to use cherry-pick and fix merge conflicts.

Checkpoint 4
- git switch -c experiment/fterrone 
- git add.
- git commit -m "add a comment"
- git branch -D experiment/fterrone              
- git reflog                                     
- git switch -c recovered/fterrone  2be781c      
- git switch feature/fterrone                    
- git merge recovered/fterrone 
- git_project_1 % git log    
 
Checkpoint 4 taught me how to recover a deleted branch by using reflog. It also taught me how to merge two branches.

Checkpoint 6

- git rebase -i main       
- git push --force-with-lease

This checkpoint taught me how to use the rebase-interactive editor to clean up and improve the commit history.

checkpoint 7
- git add .
- git commit -m "add comments to validate_operation and added Learning files"
- git rebase -i main       
- git push --force-with-lease
This check point helped me learn to give feed back on poll request. it also allowed me to apllay how to handel feed back.
