# Day 3 - Git Repository, Staging & Commit


## 1.What is a Git Repository?
   A Git repository is a directory where Git tracks the changes of files and stores the project's history.


## 2.Initialize a Git Repository
   git init : git init creates a hidden .git directory. This directory contains the Git repository's internal information like config files,objects,HEAD etc.

## 3.Git Workflow

             Working Directory
                     │
                     │ git add
                     ↓
               Staging Area
                     │
                     │ git commit
                     ↓
              Local Repository
                     │
                     │ git push
                     ↓
             Remote Repository
                  (GitHub)



## 4.Check Repository Status
   git status : this command will give you the state of the working directory and staging area.
   *Untracked
   *Modified
   *Stagged

## 5.Adding Files to the Staging Area
   * git add filename : this command will move the specific file mentioned from working directory to staging area
   * git add . : this command will add all the files from working directory to staging area including hidden files.

## 6.Remove a File from the Staging Area/Make a file untracked
   * git rm --cached filename : this command will move the file from staging area to working directory

## 7. Creating a Commit 
   * git commit -m "adding the files to local repository" : This command will help the files to move from stagging area to local repository
  
   * git commit --amend -m "message"  : This command will modify the latest commit id message and a new commit id will be formed with the new commit message.

   
 ## 8.View Commit History
    * git log : this command will list all the commits
    * git log --oneline : this command will give you the compact versions of the commit id and the commit message.
    * git log --oneline --graph : This will give the commits in a graphical manner
    * git log --oneline --graph --all
    * git reflog : will list the deleted commit ids/ Previous  positions of head
    * git show <Commit_id> : this will show all the information related to give commit id.
    * git log --oneline -- filename : This command will give you the list of commit ids related to one file.


## 9.View Unstaged and Staged Changes
   * git diff : This displays the differences between the Working Directory and the Staging Area.
   * git diff --staged This displays the differences between the Staging Area and the latest commit.



