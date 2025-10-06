git --version
git config --global user.name "username"
git config --global user.email "user email"
git config --list


cd <-dir name->
git clone <-copied address of repo->
ls
ls -force
ls -h
git status
git add "file name"
git add .

git commit -m "some message"

git push origin main

git init 								#to make git track the dir if not already eg after creating new dir by mkdir


git remote add origin <-link>
git remote -v
git branch
git branch -M main 						#to rename branch to main if required
git push origin main					#to push to origin main
git push -u origin main 				#(to permanently use origin branch

git checkout <-branch name-> 			#to navigate
git checkout -b <-new branch name->		#to create new branch
git branch -d <-branch name-> 			#to delete branch


#MERGING CODE
git diff <-branch name->				#to compare commits, branches, files and more
git merge <-branch name->				#to merge 2 branches

#PULL COMMAND
git pull origin main					#download from remote and update the local and match


#UNDOING CHANGES
#stages changes:
git reset <-file name->
git reset
#commited changes:
git reset HEAD~1
#commited changes for many commits
git reset <-commit hash->
git reset --hard <-commit hash->

git log									#to check and copy hash