
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

    


