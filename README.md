
# Version control with git bash and GitHub

## Introduction

*Version Control* : Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

*Git Bash* : Its command line interface to access git

*GitHub* : Hosting platform for collaboration

## Getting Started

### Requirement

1. A GitHub account from [GitHub](https://github.com/)
2. Git bash setup from [GIT_SCM](https://git-scm.com/downloads)

### Create a repository

1. Create a new repository by clicking on new button on you GitHub dashboard fill up the form to create a remote repository
2. Instruction for initializing the repository then will appear

### Setting up Git Bash

1.	Start git bash from by searching in search box
2.	Add user email and username to the git bash using following commands
    - git config --global user.name "your_username"
    - git config --global user.email "MY_NAME@example.com

### Initializing Local repository

1. Create a folder in you local machine
2. Right click on or inside folder and select “Open Git bash here”
3. Paste the commands in instruction from github
    - `echo "# test-giit" >> README.md `
    : This command will add text in readme markdown file of our repository
    - `git init`
    : This command is used to initialize a local repository
    - `git add README.md`
    : This will add the specific file into our commit
    - `git commit -m "first commit"`
    : This will add a label to our commit
    - `git branch -M main`
    : This will set current branch to main branch
    - `git remote add origin git@github.com:username/repository_name.git`
    : This will set remote repository’s address as local repository
    - `git push -u origin main`
    : This will push current commits in local repository to main branch of remote repository
4. After running the command popup for credential verification will appear select “Open in browser” to continue verification from you GitHub account

### Error and solution

> Error : Please make sure you have the correct access rights and the repository exists.   
Error At : Initializing local repository

> Solution Change the Git URL in local repository

`git remote set-url origin https://github.com/username/repository.git`

### Cloning a existing repository

`Git clone  https://github.com/username/repository-name.git`
: By using above command a new repository can be cloned to local environment 

### Creating branch

Branches are forked repositories where development  is done by individual developer before incorporating the changes to upstream repository  

`Git branch branch_name`
: By using this command you can create a new branch locally  

`Git checkout branch_name`
: By using this command git will switch to that branch and it will show as current branch any changes committed will be for this branch only

### Checking status

Any changes made to code base will create new changes in local repository changes made can be seen by command  

`Git status`
: This will show file name in which changes are created shown in red also any changes finalized will show in green which are ready to be committed

### Staging changes to commit

Any changes made in codebase needs to be committed or removed from the git repository before updating it with remote repository  

`Git add <file>`
: This will add all changes made in specific file to staging  

`Git restore <file>`
: This will discard changes made in specific file  

`Git add .`
: This will add all changes made to repository to staging   

### Gitignore

*gitignore* is a file located in folder structure which specifies intentionally untracked files that git should ignore. Once a file added in *gitignore* any changes made to it will not show up in git status command. Files such as config, env variables or large files are added in *gitignore*

### Creating a local commit

In order to push local changes to remote repository committing changes is necessary which then can be pushed to remote repository  

`Git commit -m “name of the  commit”`
: This command will create new commit with all the staged changes, -m flag will be used to add commit message

### Pushing commits to remote
All changes done are only on local machine only pushing them to remote repository is necessary  

`Git push origin branch_name`
: This command will push any changes created to remote git repository branch of the same name  

### Pull request
You can pull commits from any branch using pull request and used to be up to date with other developers code  

`Git pull origin branch_name`
: Pull codebase on branch_name to owners branch






