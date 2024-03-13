# lab-MST
4. The task
You again live in your own branch, this time we will be doing a bit of juggling with branches, to show how lightweight branches are in git. Hint: git switch will make you switch from one branch to another.
1.	Use git branch to see the two branches that are relevant for this exercise
   $ git branch
2.	What branch are you on?
   I am on test branch
3.	Use git branch mybranch to create a new branch called mybranch
   $ git branch mybranch
4.	Use git branch again to see the new branch created.
   $ git branch
5.	Use git switch mybranch to switch to your new branch.
   $ git checkout mybranch
6.	How does the output from git status change when you switch between the master and the new branch that you have created?
   $ git status
7.	How does the workspace change when you change between the two branches?
   $ git checkout <branch_name> can be used to switch between branches
  	nothing done on feature branch will affect the master branch unless
  	$ git merge <branch name> is used to merge the changes.
8.	Make sure you are on your mybranch branch before you continue.
   $ git checkout mybranch
9.	Create a file called file1.txt with your name.
    $ touch file1.txt
  	$ vi file1.txt
  	$ cat file1.txt
10.	Add the file and commit with this change.
    $ git add file1.txt
   	$ git commit -m "commited file1.txt"
11.	Use git log --oneline --graph to see your branch pointing to the new commit.
    $ git log --oneline --graph
12.	Switch back to the branch called master.
    $ git checkout master
13.	Use git log --oneline --graph and notice how the commit you made on the mybranch branch is missing on the master branch.
    $ git log --oneline --graph
14.	Make a new file called file2.txt and commit that file.
  	$ git touch file2.txt
    $ git add file2.txt
   	$ git commit -m "commited file2.txt"
15.	Use git log --oneline --graph --all to see your branch pointing to the new commit, and that the two branches now have different commits on them.
    $ git log --oneline --graph
16.	Switch to your branch mybranch.
    $ git checkout mybranch
17.	What happened to your working directory? Can you see your file2.txt?
    $ pwd
   	$ ls
18.	Use git diff mybranch master to see the difference between the two branches.
    $ git diff mybranch master
