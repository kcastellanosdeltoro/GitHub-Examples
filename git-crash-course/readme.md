## Git Hidden Folder

There is a hidden folder called `.git` which tells you that your project is git repo.

If we wanted to create a new repo in a new project we create the folder and initalize that repo using.
```sh
/workspaces/tmp/ mkdir new-project
/workspaces/tmp/ cd new-project
/workspaces/tmp/new-prjoect git init
/workspaces/tmp/new-prjoect touch readme.md
/workspaces/tmp/new-prjoect code readme.md
/workspaces/tmp/new-prjoect git status
/workspaces/tmp/new-prjoect git add readme.md
/workspaces/tmp/new-prjoect git commit -m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH and GitHub CLI.

Since we are using GitHub Codespace we will create a temporary directory in our workspace.

```sh
workspaces/GitHub-Examples (main) $ cd ..
/workspaces $ mkdir tmp
/workspaces $ cd tmp
/workspaces/tmp $
```

## HTTPS
```sh
git clone https://github.com/kcastellanosdeltoro/GitHub-Examples.git
```

## SSH
You need SSH Key in your device pairing in GitHub
```sh
git clone git@github.com:kcastellanosdeltoro/GitHub-Examples.git
```
## Add
Following command allow us add file to Staged.
`git add namefile.txt`

Following command allow us add all possible files.
`git add .`

## Commits
When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.
```sh
git commit
```
Set the global editor
```sh
git config --global core.editor emacs
```
Make a commit and commit message without opening the editor
```sh
git commit -m "message"
```

## Branches

## Remotes

## Merging 

## Reset
Reset allows you to move Staged Changes to be Unstaged.

This command is so useful you to revert all files not be commited.
```sh
git add .
git reset
```
>"git reset" will revert "git add ." remember this command put all files in Staged.

## Status
The following command permitted allow us to view what files will commited or not commited.
```sh
git status
```
## Gitconfig file

The gitconfig file is what stores your global configurations for git sush as email, name, editor and more.
```sh
git config --list 
```

When you first install git on a machine you are suppose to set up your name and email
```sh
git config --global user.name "example"
git config --global user.emial example@example.com

## Git Log
If you need the view recents commit of git tree(history)
```sh
git log
```

## Push
When we want to push a repo to our remote origin
```sh
git push
```