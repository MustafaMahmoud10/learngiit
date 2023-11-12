Git configuration



to set the name use
git config --global user.name "Name"

to set the email use 
git config --global user.email "Email"

to show your config use
git config -- list
________________________

Starting a project 

Create a local repository to tracks versions (.git) use, Everything starts from here.
git init 

to show modified files in WD, staged for your next commit (show the state of the WD and index ), use
git status 
______________________

Local changes and commited 

to add the files to the staging area use
git add [filename1] [filename2] 
to add all files to the staging area use
git add --all

git add . 

unstage file / to remove this file from staging area and return it to WD use 
git reset [filename1]

commit your staged files as snapshot as new version
git commit -m "[change desciption]"

git commit -a -m "[change desciption]"
You can add and commit tracked files with a single command by using the -a and -m options.(skip the staging area)
git log 
This command shows the commits history for the current repository
git log --oneline

git show [Commit_Id]
This command shows a specific commit.
git diff [Commit_Id] [Commit_Id]
_______________________

Branching 

to create branch ues
git branch [branch name]

to list branches ues
git branch --list

to rename branch use
git branch -m [old branch name] [new branch name]

to rename this branch 
git branch -M "rename this branch"

to delete branch use 
git branch -d[branch name]

to delete a remote branch use
git push [alias] -delete [branch name]

to add remote for repo 
git remote add [AliasVar/short_remote_name] [remote URL]

git remote
git remote -v   //verbose

to Update remote server to equl local  use
git push -u [AliasVar/remote name] [Branch name]

to Update local to equl remote server  use
git pull [AliasVar/remote name] [Branch name]

to rename remote server use
git remote rename [old name] [new name] 

to remove remote server use
git remote rm [AliasVar/remote name]





git revert


git reset --[mode] [Commit_Id]
git reset --hard 6588393

mode
mixed This is the default mode , return commits to WD
hard delete commits 
soft return commits to staging area 



Note :-
 git revert is a “safe” way to undo changes, you can think of git reset as the dangerous method
 revert work in remote reset work in local 
 reset move head and master pointer to specific Commit_Id , history is effective (history بتغير في ال )



git mv oldfile newfile
This command to git mv oldfile newfile 
git rm filename
this command to remove tracked files from the current working tree in Git



git push --delete [AliasVar/remote name] [Branch name]
this command to remove a remote branch in Git:



   clone     Clone a repository into a new directory
   init     





    add       Add file contents to the index



  fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects
