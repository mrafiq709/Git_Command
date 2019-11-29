# Git_Command
Essential git Command

#For adding Remote:
---------------------
    git remote add origin <remote_repo>

#For adding all Files:
----------------------
    git add .

#For Commit:
----------------------
    git commit -m "Initial Commit"

#If Remote is already exist:
-------------------------------
    git remote set-url origin <remote_repo>
    git remote -v

#For Exception:
------------------
    git pull origin master --allow-unrelated-histories

#for marge conflict:
------------------------
    git commit -a
    [Warning !!! Before Pushing Solve the merge conflict manually and then again commit -> then push]

#for  "! [rejected]        master -> master (non-fast-forward)"
--------------------------------------------------------------------
    git pull origin master
    git fetch origin
    git merge origin/master
    git pull --rebase origin master
    git push origin master
    
#for  "! [rejected]        brach -> branch (non-fast-forward)"
--------------------------------------------------------------------
<a href="https://imgur.com/jirwHNM"><img src="https://i.imgur.com/jirwHNM.png" title="source: imgur.com" /></a><br/><br/>

    git fetch origin
    git fetch origin branch_name
    git merge/branch_name
    
    Then solve merge conflict and commit.
    
#Forcely push:
------------------------------
    git push --force origin master
    
#For set Username and Email:
-----------------------------
    git config --global user.name "user_name"
    git config --global user.email "user_email"
    git remote rm origin

#For Branch Create:
--------------------
    git checkout -b <branch-name>
    git pull origin <branch-name>
    
#For Brance Clone:
--------------------
    git clone -b <branch-name> <remote_repo>

#For Branch Rename:
------------------------------
    git branch -m new_branch /* Current branch will be rename locally */
    git push --set-upstream origin new_branch /* Push the new branch, set local branch to track the new remote */

#For Branch Delete:
-------------------------
    git push origin --delete <branch-name>
    
#fatal: refusing to merge unrelated histories:
------------------------------------------------
    git pull origin branchname --allow-unrelated-histories

#Delete Recently Pull Request:
-----------------------------------
    git reset --hard HEAD^1
    
#If you want to see what you haven't git added yet:
-----------------------------------------------------
    git diff myfile.txt
    
#Already added changes
-----------------------
    git diff --cached myfile.txt

#Will show you changes you added to your worktree from the last commit:
----------------------------------------------------------------------------
    git diff HEAD file
