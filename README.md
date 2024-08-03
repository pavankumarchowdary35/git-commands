# Important Commands

## Git Configurations

Git configurations are settings that allow you to customize how Git works. They consist of variables and their values, and they are stored in a couple of different files. To work with Git, you must set a few configuration variables related to user settings.

```
git version
git config --global --list
git config --global user.name "nachiketh"
git config --global user.email "support@manifoldailearning.in"
git config --global init.defaultBranch main
git config --global --list

```

## Working with Local Repo

```
git init
git status
git add file1.py
git status
git commit -m "myfirst commit"
git status
git log
```
## Working with Branches

```
git branch
git branch dev
git log
git branch
```

## Switching the Branches

```
git switch dev
git checkout dev
# updated the source code
git add . 
git commit -m "v3"
git log
git checkout main
```

## Fast Forward merging
```
#create v4 in dev & commit to the repo
git switch main
git merge dev
```

## Git Checkouts

```
git checkout <commit-hash>
git checkout -b feature
git switch -c featurev2
```

## Remote Git Repositories

```
#create remote repo
git remote add origin <url>
git remote
git remote -v
git push origin main
git branch --all
```

## Cloning and Delete Branches
```
git clone <url> <dir-name>
git clone https://github.com/manifoldailearning/git4mlops.git my-folder
cd my-folder
git branch --all
git checkout -b unit-test
git push -u origin unit-test
git checkout main
git branch -d <branch-name> #delete local branch
git branch -d unit-test
git push origin -d unit-test
git branch --all
```