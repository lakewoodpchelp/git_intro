## This example is bash environment under Windows 10 pro. 

##1  How to create a clean/empty local git repository?  
super@DESKTOP-DLLM5NQ:~/python$ mkdir git_intro
super@DESKTOP-DLLM5NQ:~/python$ cd git_intro/
super@DESKTOP-DLLM5NQ:~/python/git_intro$ ls -altr
total 0
drwxr-xr-x 1 super super 512 Jul 12 16:07 ..
drwxr-xr-x 1 super super 512 Jul 12 16:07 .
super@DESKTOP-DLLM5NQ:~/python/git_intro$ git init
Initialized empty Git repository in /home/super/python/git_intro/.git/

super@DESKTOP-DLLM5NQ:~/python/git_intro$ ls -altr .git
total 0
drwxr-xr-x 1 super super 512 Jul 12 16:08 branches
drwxr-xr-x 1 super super 512 Jul 12 16:08 ..
-rw-r--r-- 1 super super  73 Jul 12 16:08 description
drwxr-xr-x 1 super super 512 Jul 12 16:08 info
drwxr-xr-x 1 super super 512 Jul 12 16:08 hooks
drwxr-xr-x 1 super super 512 Jul 12 16:08 refs
-rw-r--r-- 1 super super  23 Jul 12 16:08 HEAD
-rw-r--r-- 1 super super  92 Jul 12 16:08 config
drwxr-xr-x 1 super super 512 Jul 12 16:08 objects
drwxr-xr-x 1 super super 512 Jul 12 16:08 .

##The git directory contains all the changes and their history and the working tree contains the current versions of the files

##  Staging area (index) -- A file maintained by Git that contains all of the information about what files and changes are going to go into your next commit
##2  add a file to git working tree  
git add git_introduction.txt
git status 
git commit 
git status 


##3  What's the difference of tracked and untracked file?  Tracked file status: modified, staged or committed:
##4  Git enforces commit messages. Empty commit message will make the commit to be aborted. 
##5  Commit message should be a short description of the change (up to 50 characters), followed by one or more paragrphs giving more details of the change. Each line is kept under 72 characters in length  
##6  Head is the alias to the currently checked up snapshot of your project.  All commands run based on HEAD. 
##7  git log has many more option to see patch, specific commit, et al
# 	git log -p 
# 	git log -p -n 1 

##8  git diff  
#	git diff --staged  
 
## view difference between staged with --cached or --staged 
git diff --staged 
