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
git push -u origin main 				#to permanently use origin branch

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



You can create a GitHub repository and push your existing VS Code project by following these steps:
### Create GitHub Repository
Go to GitHub.com and create a new empty repository. Do not initialize it with README, license, or gitignore files to avoid conflicts. Copy the repository URL from the Quick Setup page.
### Initialize Git Locally
git init
### Stage and Commit Files
git add .
git commit -m "Initial commit"
### Connect to GitHub
git remote add origin https://github.com/yourusername/yourrepository.git
git remote -v
### Push to GitHub
git push -u origin main
If your default branch is named "master" instead of "main", replace "main" with "master". The `-u` flag sets the upstream branch for future pushes.
