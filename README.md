# git-operation
## Basics of Git
1. git init - initialise the repository 
2. git add <file-name or repository-name> or git add . - for adding the files to the staging area
3. git commit -m message - commiting the file with a message. It is simply snapshot of the project i.e it gives the generally what is happening or happened    to the file at particular time.
4. git reset -undoing local commits

## Branching and Merging stufff
1. git checkout -b <branch_name> - make the new branch and switch to that branch immediately
2. git checkout main - switch to the main branch
3. git merge <branch_name> commit -m <commit-message> -merge the branch with the main
4. git rebase <branch_name> - similar to the merge but it gives all the commit point from the branch and merges it with main branch which helps you to  debug.
5. git cherry-pick <commit-id> -picking one commit from a branch and apply to another

## Intermediate Git Operations
### Stash - Storing the uncommited changes
1. git stash - temporarily and safely store the uncommited local changes 
2. git stash list stash@{i} - gives the list of stashed changes and here i is the index of the squashed changes
3. git stash apply - stash changes back and it preserves the stash in the stash list
4. git stash pop - stash changes back but it doesn't keep the stash and deletes one by one once it gets executed

## Squash - Combining difference commits to the one single commit 
### Steps:
1. git rebase -i HEAD~N where N is the no of recent commits and 'i' is interactive mode
2. In editor change the mode to squash from another 
3. save and exit 

