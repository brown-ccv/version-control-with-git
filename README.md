# Version Control with Git
A practical introduction to version control using Git. In this workshop we cover 

* creating a repository
* checking the status of a repository
* committing changes
* viewing and undoing changes
* reverting to older versions of files
* setting up a remote repository on github 

The workshop presentation slides with exercies can be viewed at 

[google slide deck](https://docs.google.com/presentation/d/1fkSbqLP3ipCPDsUIWRaEb6N8JzCOuGjL_iFqqRAFgBA/edit?usp=sharing)

You can attend this workshop in person. To find upcoming CCV events visit:

[events.brown.edu/ccv](https://events.brown.edu/ccv/view/month)

The aim of the workshop is to get you started using version control, which is a great skill to have as you develop code, scripts, and even your thesis.  <em>Anything</em> that you edit can benefit from version control.  Version control allows you to recover previous versions of your project, and it allows multiple people to work on the same documents. Git is an extremely powerful tool for version control, which you can start using in a simple way to make your life easier.

## Important Concepts

#### Hidden files
Files that start with a . are hidden.  There are two to be aware of for this workshop

    ~/.gitconfig

    .gitignore

To view hidden files in a directory, use
`ls -a`

#### Git stores a snapshot of your project

Your project in git is stored in a **repository**

Working on a project with git follows this pattern:

<em>Edit / add / commit </em>

 * Edit your files with your new amazing science (this bit is up to you).

 * `git add` - add a change to the staging area.   

 * `git commit`  - take a snapshot of the project


#### Github 

Github is a place online to store your git repositories, with some social media aspects. 
There are other services you can use, for example [bitbucket](https://www.bitbucket.org) and [gitlab](https://about.gitlab.com/). 

#### Git terminolgy

`clone` - copy a respository to your computer so you can work on it

`fork` - copy a respotiory for independent development

`commit` - make a snapshot of the repository

`branch` - branch off from the main developement to work on something


#### Git - where am I?

`git log` - see what commit you're on

`git remote -v` - see what remote repository you are tracking

`git branch` - find out what branch you are on


#### Viewing your changes

`git status` - see any edits you made

`git diff` - show difference between your files and the commited files

`git diff --cached`  same as diff, but for files you have already added


#### Reverting changes

`git log --oneline`  - a condense way to view the log

`git revert` - undo history but keep a record

`git reset`   - undo history like it never happened **Beware**

#### Working with remotes

`git pull` - get changes from the remote repository

`git push origin master` - send your changes up to the remote repository

##### Storing local changes while you pull from a remote repository

Some times the changes you pull from a remote repository will conflict with your local changes.  You can stash your local changes, pull the new changes from the remote repository, then pop your changes back. 

`git stash`

`git stash pop`


## Git commands used in this workshop

`git init`

`git add`

`git status`

`git commit`

`git log`

`git log --oneline`

`git remote add origin https://github.com/…….`

`git push origin master`

`git checkout “commit#” “file”`

`git clone https://github.com/…….`

`git pull`

`git difftool --tool=xxdiff`

----
Checkout other [workshops](https://brownhpc.github.io/) offered by the CCV HPC team.

To sign up for live events, go to the [CCV Events Calendar](https://events.brown.edu/ccv/view/all)
