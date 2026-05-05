## Cloning 
Since we're simulating making a local repo, we need to clone the repo in a folder. There is a hidden folder `.git` which tells you this is a git repo.

```bash
mkdir /workspaces/tmp
cd /workspaces/tmp 
```

If we wanted to create a git repo in a new project, we must initialize it

```bash
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
code Readme.md
open Readme.md
git add .
# make changes to the file
git commit -m "add new readme file"
```

## HTTPS  
```bash
git clone https://github.com/nickv893/Github-Examples.git
```

### Add
Add changed files to the staged, add . stages all

```bash
git add .
git add Readme.md
```

### Status
Git status shows what files will or won't be commited.

```bash
git status
```

### Reset
Allows you to revert staged files back to unstaged

```bash
git add . 
git reset
```

## Gitconfig file
The gitconfig file is waht stores your global configurations for git such as email, name, editor and more.

```bash
git config --list
```

When you first install Git on a machine you are supposed to set up your name and email


### Commit
Make a commit and commit message without opening editor

```bash
git commit -m "added another exclamation"
```

### Log
git log will show recent git commits to git tree

### Push
When we want to push a repo to our remote origin

```bash
git push
```