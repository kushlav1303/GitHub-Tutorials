## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our profject is a git repo

If we want to create a git repo in a new project, we would create the folder and initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
# make changes to Readme.md
git status
git add .
git comit -a -m "add readme file"
```

### Cloning

We can clone 3 ways: HTTPS, SH, Github CLI

We are using Github Codespaces, so we'll create temp directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/kushlav1303/GitHub-Tutorials.git
```

## Commits

When we want to commit code, we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

Make a commit and commit message withouth opening an editor

```sh
git commit -m "add another exclamation mark"
```

## Branches

List of branches
```
git branch
```

Create a new branch
```
git branch <<branch-name>>
```

Checkout the branch
```
git checkout <<branch-name>>
```

## Remotes

## Stashing

## Merging

## Add

When we want to stage changed that we want to included in the commit.
We can use . to add all the files to staging area

```
git add Readme.md
fir add .
```

## Reset

Reset allows you to move staged changes to be unstaged.
This is useful when you want to revert all files so that they not commit 

```
git add .
git reset
```

> git reset will revert a git add .

## Status

Git status shows you what files will or will not be commited

```
git status
```

## Gitconfig file

The gitconfig file is what stores your global configurations for git such as email, name, editor and more

Showing contens of out .gitconfig file

```sh
git config --list
```

When you install git on a machine, you are supposed to setup yor name and email

```sh
git config --global user.name "kushlav1303"
git config --global user.email "kushlav@gmail.com"
```

## Log

git log will show recent git commits to the git tree

## Push

When we want to push a repo to our remote repo

```
git push
```