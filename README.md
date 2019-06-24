# Git_Command
Essential git Command

#For adding Remote:
---------------------
    git remote add origin https://github.com/rafiq-istvn/XamarinApps.git

#For adding all Files:
----------------------
    git add .

#For Commit:
----------------------
    git commit -m "Initial Commit"

#If Remote is already exist:
-------------------------------
    git remote set-url origin https://github.com/rafiq-istvn/XamarinApps.git
    git remote -v

#For Exception:
------------------
    git pull origin master --allow-unrelated-histories

#for marge conflict:
------------------------
    git commit -a

#for  "! [rejected]        master -> master (non-fast-forward)"
--------------------------------------------------------------------
`
    git pull origin master
    git fetch origin
    git merge origin/master
    git pull --rebase origin master
    git push origin master
`
    
#For set Username and Email:
-----------------------------
    git config --global user.name "mrafiq709"
    git config --global user.email "mrafiq709@gmail.com"
    git remote rm origin

#For Branch:
--------------------
    git checkout -b AppLifeCycle
    git pull origin AppLifeCycle

#For Branch Rename:
------------------------------
    git branch -m new_branch /* Current branch will be rename locally */
    git push --set-upstream origin new_branch /* Push the new branch, set local branch to track the new remote */

#For Branch Delete:
-------------------------
    git push origin --delete <branch>
