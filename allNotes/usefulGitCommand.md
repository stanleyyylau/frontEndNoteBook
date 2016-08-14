# Git commands that are useful

[Git commands That I use yesterday](https://medium.freecodecamp.com/git-cheat-sheet-and-best-practices-c6ce5321f52#.1uuec8v48)

## Most basic
```
git add --all
git commit -am "<message>"
git push origin master

```

## Regularly used commands
```
git init

```
+ The default name (also known as an alias) for your **remote** repo is **origin**
+ If you copy a project from Github, you can use **git remote -v** to view its origin URL
+ Use **git remote add origin <URL>** to associate your local repo to Github repo
+ If you copy a repo from someone else and want to make it your own
```
git remote -v
git remote add origin <url>
git remote set-url origin <url>

```
+ Using **Git clone <url>** alone means you will not be able to push to GitHub until you change the origin using the commands above

## Start using branches
+ The command **git branch** lists all branches on your local machine
+ To create a new branch, you can use **git branch <name>**
+ The **git checkout <name>** command switches to an existing branch
+ **git checkout -b <name>** to create a branch and switch to it
+ You use the **git merge <branch>** command to merge the branch you specify with your current branch
+ Use **git pull origin <branch>** to pull the most recent changes from that remote branch
+ Use **git status** and **git diff --stat** to see the number of lines changed in each file

## Advanced commands and best practices
