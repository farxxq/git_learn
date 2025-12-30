# git_learn
Git Commands

1. Initializaiton :
    ### git init
2. Adding initial data to tracked path:
    ### git add .
    `NOTE: git add (folder/filename)... If '.', then it saves all of the changed files`
3. Commit the changes to local repo: 
    ### git commit -m "my first commit"
    `NOTE: git commit -m "()" (commit message within quotes)...`
4. Adding the remote github to the folder: 
    ### git remote add origin https://github.com/farxxq/git_learn.git
    `NOTE: git remote add origin (repoLink)...`
5. Setting the default branch from master to main: 
    ### git branch -M main
    `NOTE: git branch -M main (the default initialized branch in local git is master whereas the branch in the remote is main so we change the local git branch also to main)...`
6. Saving the changes to the github: 
    ### git push -u origin main
     `NOTE: git push -u origin (branch_name) (save the changes to the main branch), (-u origin main: makes the main branch as the active one,then each time we push it gets saved to this branch and we need to have use this term later on)...`


Additional commands:

1. check the status of the current folder: 
    ### git status
    `NOTE: git status - is responsible to show the status of the git working tree`



