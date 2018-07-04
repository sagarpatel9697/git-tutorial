# git-tutorial
Topics of learning git and github in simple way.

## Getting Started

### Prerequisites

- GIT installed on your machine. If not, you can download it from [official site](https://git-scm.com/downloads)
- Account on [github.com](https://github.com/)

## Why to use GIT ?

1. What was a challanges for developers?

![Challanges in earlier days](./images/tutorial_1.jpg)

2. What was another solution?

![Another solution](./images/tutorial_2.jpg)

3. What to do now?

![what to do now](./images/tutorial_3.jpg)

4. Version Control System

![VCS](./images/tutorial_4.jpg)

## Introduction

* [What is GIT](#what-is-git)
* [What is GITHUB](#what-is-github)
* [Is GIT related to GITHUB](#is-git-related-to-github)
* [A simple workflow](#a-simple-workflow)


### What is GIT
- VCS (Version Control System)
- track files/folders
- to work in team
- free and opensource

Two types of VCS
1. Centralized version control

![CVCS](./images/cvcs.jpg)

2. Distributed version control

![DVCS](./images/dvcs.jpg)

``GIT = DVCS``


### What is GITHUB

- Website/Server to upload repository
- Backup funnctionality
- GUI for repo
- Manage team

### Is GIT related to GITHUB

NO !!!!!!
GIT can also be used with others repository management system like bitbucket.

### A simple workflow

![GIT Workflow](./images/workflow.jpg)

## Setup Repository

1. Run `git init` command
2. Add project files to folder and adding it to stage area via `git add` command
3. Commit staged files with `git commit -m <Message>` command
4. Link remote repository with local using `git remote add origin <repo url>` command
5. Push all local repository commits to remote `git push`


## Branching

1. what are branches & commands?
- Feature/Task wise branch
- commands for create, checkout, merge & delete

#### Create Branch

`git branch <branch name>`

you're still on ``master`` branch so for adding new features, you have to swicth on newly created branch. Follow next **checkout** step.

#### Checkout Branch

`git checkout <branch name>`

Add new fetaures in your working repo and push it on remote repo. Now you can see new branch in branch list of github.

#### Merge Branch

`git merge <source branch name>`

Add new fetaures in your working repo and push it on remote repo. Now you can see new branch in branch list of github.

#### Delete Branch

`git branch -d <branch name>` - From local repo

`git push origin -d <branch name>` - From remote repo

## Tags/Releases

Specific points in history for repository called as release or versions.

### Create Tag

Cretae tag in local repository

`git tag <tag name>`

### Show Tag(s)

Show list of tags in local repository

`git tag`

`git show <tag name>`

### Push Tag

Push tag to remote repository

`git push origin <tag name>`

### Delete Tag

Delete tag from repository

`git tag -d <tag name>` - From local repo

`git push origin -d <tag name>` - From remote repo


#### Checkout Tag

No concept for checkout tags, but if you want it then you can create a branch with specific tag

`git checkout -b <branch name> <tag name>`

