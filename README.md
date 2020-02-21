# Version Control with Git.  Feb 2020
A practical introduction to version control using Git. Topics covered include: 

* creating a repository
* checking the status of a repository
* committing changes, viewing changes
* reverting to older versions of files
* setting up a remote repository

[Jump to Exercises](#Exercises)
 

## Important Concepts

#### Hidden files
Files that start with a . are hidden.  There are two to be aware of for this workshop

    ~/.gitconfig

    .gitignore

To view hidden files in a directory, use
`ls -l`

#### Git stores a snapshot of your project



##### Github 

Github is a place online to store your git repositories, with some social media aspects. 
There are other services you can use, for example bitbucket and gitlab. 


#### Git terminolgy

`clone` - copy a respository to your computer so you can work on it

`fork` - copy a respotiory for independent development

`commit` - make a snapshot of the repository

`branch` - branch off from the main developement to work on something


#### Git - where am I?

`git log` - see what commit you're on

`git remote` - see what remote repository you are tracking

`git branch` - find out what branch you are on


#### Viewing your changes

`git status` - see any edits you made


`git diff` - show difference between your files and the commited files

`git diff --cached`  same as diff, but for files you have already add


#### Reverting changes

`git log --oneline`  - a condense way to view the log

`git revert` - undo history but keep a record

`git reset`   - undo history like it never happened


#### Storing local changes while you pull from a remote repository

`git stash`

`git stash list`

`git stash pop`



## Git commands used in this workshop

`git init`

`git add`

`git status`

`git commit`

`git log`

`git log --oneline`

`git remote add origin https://github.com/…….`

`git push`

`git checkout`

`git checkout “commit#” “file”`

`git clone https://github.com/…….`

`git pull`

`git difftool --tool=xxdiff`

# Exercises

Initialize a repository

`git init`

Add files to a repository

`git add` 

Create a .gitingore file to tell git files not to track.  For example, your .gitingore file may look like this:

````
# files for git it ignore
*.log
*.o
*.mod
*.pyc
````

This means git will ignore any files that end in .log, .o, .mod, or .pyc

Check the status of your repository:

`git status`

Add your .gitingore file.

`git add .gitignore`

Commit a snapshot of your repository:

`git commit`

View the log

`git log`

`git log --online`

A nice tutorial on git log: https://www.atlassian.com/git/tutorials/git-log

Make a change to .gitingore, e.g. remove a line or add something. Add and commit the change

`git add .gitignore`

`git commit`

Revert the change

Find the commit to revert to

`git log` 

Revert the change

`git revert HEAD~1` 

A nice tutorial on reset, checkout and revert: https://www.atlassian.com/git/tutorials/resetting-checking-out-and-reverting







