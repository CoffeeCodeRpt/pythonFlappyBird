# Git Instructions

## Git clone

This will clone the repo to your local environment

```powershell
git clone https://github.com/CoffeeCodeRpt/pythonFlappyBird.git
```

## Create new branch

When you take on a new feature, bug, or something you want to add, you will
create a branch to work in that will be merged back into `main`. 

The first command creates the branch and the second creates a linked branch in
the repo on GitHub to push to. Replace `<branchname>` with the branch name you
decide. 

I usually make my branch names in a format I can reuse. E.g. `username-ghi0000`.
This format would be my username dash ghi = GitHub Issue and the actual issue id
number.

```powershell
git checkout -b <branchname>

git push --set-upstream origin '<branchname>'
```

## Commit and push changes to GitHub

When you have changes you want to keep, push them up to GitHub to be able to
share or create a Pull Request into `main`.

```powershell
# add all the files you have changed.
# If you only want specific files added, replace the '*' with a file name
git add *

# Commit changes with a message about your changes. This is to keep a record of changes.
# Try and make your messages informative in case we need to investigate where changes were made later on
git commit -m 'Enter commit message between single or double quotes'

# Push changes to GitHub
git push
```
