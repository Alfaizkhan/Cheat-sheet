# Cheat-sheet

# GIT Cheat Sheet

 

1) init — Create an empty GIT repository in your development directory

Go to directory
git init
 

2) status — Show the current state of the repository including un-added and un-committed files

git status
 

3) add — Add a file to the repository staging area

Create a file, e.g. file.txt
git add file.txt
Add all new or changed files to the repository staging area (the period means all)

git add .
 

4)commit — Commit all changes to the repository for first time (-m means message)

git commit –m “Initial commit”
Commit all changes to the repository for later activities

git commit –m “Description of changes being made to project”
 

5) branch — Create a new branch of the project

Choose a name for the new branch (original branch is master), e.g. test
git branch test
List all branches (* appears next to current branch)

git branch
 

6) checkout — Switch branches and check-out all files (e.g. to test branch)

git checkout test
Create a new branch and check-out files in one command

git checkout –b test
 

7) merge — Merge two branches together (go to the destination branch first, e.g. master)

git checkout master
git merge test
 

8) (delete) — Delete a branch that you no longer need (e.g. after a merge)

git branch test –d
Or to force the delete:

git branch test –D
 

9) log — View commit history (including long commit ID numbers)

git log
 

10) revert — Revert all files back to a previous commit point

git revert <long commit ID from the log command>
rm -cache

Removes cache from a specific file so that it can be added to the .gitignore
