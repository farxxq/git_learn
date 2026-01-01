# git_learn in second_branch

# #Git Commands

## Baby steps....

1. Initializaiton :
   ### `git init`
2. Adding initial data to tracked path:
   NOTE: git add (folder/filename)... If '.', then it saves all of the changed files
   ### `git add .`
3. Commit the changes to local repo:
   NOTE: git commit -m "()" (commit message within quotes)...
   ### `git commit -m "my first commit"`
4. Adding the remote github to the folder:
   NOTE: git remote add origin (repoLink)...
   ### `git remote add origin https://github.com/farxxq/(repoLink)`
5. Setting the default branch from master to main:
   NOTE: git branch -M main (the default initialized branch in local git is master whereas the branch in the remote is main so we change the local git branch also to main)...
   ### `git branch -M main`
6. Saving the changes to the github:
   NOTE: git push -u origin (branch_name) (save the changes to the main branch), 
         (-u origin main: makes the main branch as theactive one,then each time we push it gets saved to this branch and we need to have use this term later on)...
   ### `git push -u origin main`
7. Creating a branch: 
   NOTE: -> git branch - to view the branches
         -> git branch (branch_name) - to create the new branch
         -> git checkout -b (branch_name) - switches to the new branch creating it if it doesn't exist
   ### `git branch new_branch`
8. Deleting a branch: 
   NOTE: git branch -D (branch_name) - to delete an existing branch without being on that branch
   ### `git branch -D new_branch`
9. Merge the branches data:
   NOTE: git merge (branch_name) - to merge 2 branches files and data, first be active on a branch that lacks behind the changes and then use the command to merge the changes in , say branch2 to the current branch
   ### `git merge new_branch`

## Code related commands...

1. Restore file/folder data from local repo to get the last commmited changes:
   NOTE: -> git restore (file/folder_name), (To restore the unwanted changes made mistakenly)
         -> git restore --staged (file/folder_name), (To restore the file/folder pushed to stage area i.e. when it is tracked)

   ### `git restore .`

2. Revert file/folder data from the github (online)repo to get the data from one of the previous commits:
   NOTE: git revert (commit_hash_value), (To revert the unwanted changes made mistakenly),
         This will have the history of all the commits

   ### `git revert hash_value`

3. Reset command:
   NOTE: -> git reset --mixed/(no flag) HEAD~1/hash_value (To move the head to the next position and revert the data from staging and commit )
         -> git reset --soft HEAD~1/hash_value, (To move the head to the next position and revert the data without removing it from the stage area (safer))
         -> git reset --hard HEAD~1/hash_value, (To move the head to the next position and revert the data affecting the staging and working directory as well (cautious))
   ### `git reset --soft HEAD~1`

# #Additional commands:

1. check the status of the current folder:
   NOTE: git status - is responsible to show the status of the git working tree
   ### `git status`

2. check the commits in terminal:
   NOTE: -> git log - to see detailed logs of commit
         -> git log --oneline - to see the commit msg and the hash value
   ### `git log`

3. Checkout/switch command:
   NOTE: -> git checkout (branch_name) - to switch to the other existing branch
         -> git checkout -b (branch_name) - to switch to the new branch creating it if it doesn't already exist
         *> git switch (branch_name) - to switch to the other existing branch
         *> git switch -c (branch_name) - to switch to the new branch creating it if it doesn't already exist
   ### `git checkout new_branch`
   ### `git switch new_branch`
