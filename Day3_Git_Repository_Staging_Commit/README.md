What is a Git Repository?
A Git repository is a directory where Git tracks the changes of files and stores the project's history.

git init : git init creates a hidden .git directory. This directory contains the Git repository's internal information like config files,objects,HEAD etc.

             Git Workflow

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




git status : this command will give you the status of the git files

git add filename : this command will move the file from working directory to staging area

git add . : this command will moe all the files from working directory to staging area

git rm --cached filename : this command will move the file from staging area to working directory


git commit -m "adding the files to local repository"

git commit --amend -m "message"  : This command will modify the latest commit id message and a new commit id will be formed with the new commit message.

git log : this command will list the commit history

git log --oneline : this command will give you the short commit id and the commit message.

git log --oneline --graph :

git log --oneline --graph --all

git reflog : will list the deleted commit ids

git show <Commit_id>
What is a Git Repository?
A Git repository is a directory where Git tracks the changes of files and stores the project's history.

git init : git init creates a hidden .git directory. This directory contains the Git repository's internal information like config files,objects,HEAD etc.

             Git Workflow

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




git status : this command will give you the status of the git files

git add filename : this command will move the file from working directory to staging area

git add . : this command will moe all the files from working directory to staging area

git rm --cached filename : this command will move the file from staging area to working directory


git commit -m "adding the files to local repository"

git commit --amend -m "message"  : This command will modify the latest commit id message and a new commit id will be formed with the new commit message.

git log : this command will list the commit history

git log --oneline : this command will give you the short commit id and the commit message.

git log --oneline --graph :

git log --oneline --graph --all

git reflog : will list the deleted commit ids

git show <Commit_id>
git diff : It will give the information about the files in the worikng which are not yet to pushed to staging area.

warning: in the working copy of 'Day3_Git_Repository_Staging_Commit/README.md', LF will be replaced by CRLF the next time Git touches it
diff --git a/Day3_Git_Repository_Staging_Commit/README.md b/Day3_Git_Repository_Staging_Commit/README.md
index d9d9748..cec4c1f 100644
--- a/Day3_Git_Repository_Staging_Commit/README.md
+++ b/Day3_Git_Repository_Staging_Commit/README.md
@@ -43,4 +43,6 @@ git log --oneline --graph :

 git log --oneline --graph --all

+git show <Commit_id>
+


git diff --staged : this will give information about the files in the staging are and not yet comited.

git log --oneline -- filename : This command will give you the list of commit ids related to one file.

