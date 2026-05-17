# Git : 

* Git is a distributed version control system used to track changes in projects.

* Tracks changes: Every edit you make to your code (or any file) can be saved as a “version.”

* Lets you go back in time: You can restore older versions if something breaks.

* Supports collaboration: Multiple people can work on the same project without overwriting each other’s work.

* Manages branches: You can create separate “branches” to try new features safely, then merge them later.

## Why it’s called “distributed” : 

* Unlike older systems, Git doesn’t rely on a single central server. Every user has a full copy of the project and its history on their own computer.

### Features of Git : 

1. Distributed system

2. Version tracking/ controling

3. Collaboration 

4. Branching

5. Merging

# GitHub : 

* GitHub is a cloud-based platform that uses Git to help developers store, manage, track, and collaborate on software projects

# Git Workflow : 

<img width="300" height="250" alt="Git_Workflow" src="https://github.com/user-attachments/assets/ba6a99ea-59be-4ba8-a768-9689320c5b6e" />

### Branching and Merging : 

* Branching allows you to work on new features or bug fixes without affecting the main codebase. when ready, you can merge the new code into the main branch

### Commands : 

1. git status : Shows the current state of your repository.

2. git log : Displays the commit history of your Git repository.

3. git init : The git init command is used to initialize a new Git repository in a folder.
  
    * Git creates a hidden ".git" folder that stores: commit history ,branches ,configuration ,tracking information
    * After this, Git starts tracking the project.
  
4. git add : The git add command is used to move changes into the staging area before committing.
    
    * After you run :git add file.txt -> Git starts tracking that file.
    * Add all files in current folder : git add .

5. git commit -m "your message" : Save this version/changes of the project as local Repo.

6. iniliase a remote repo in github , then:
    
    * git remote add origin githubAccount/Remote_Repo.git       origin is a Alias ie short name for repo   
    * git branch -M main
    * git push -u origin main

7. git pull : someone made some changes or improved something or added a new file in the remote repository by cloning it and you want to keep those changes , use git pull to save those changes to the working directory

    * "Downloads and updates your local repository with the latest changes from the remote repository (like GitHub)" .

8. touch .gitignore : A .gitignore file tells Git: “Ignore these files/folders — don’t track or upload them.”

   * Example .gitignore
        #### Ignore log files
        *.log

        #### Ignore Python cache
       __pycache__/

        #### Ignore node modules
        node_modules/

       #### Ignore VS Code settings
       .vscode/

       #### Ignore environment variables
       .env 

## Getting code from GitHub : 

* Downloading : you can download a Zip file of the repo

* git clone : Get a copy of the full repo on to your machine

* git pull : Get the latest changes from a repo

* git fetch : Get the latest changes without merging

* forking : Copy a repository into your own GitHub account

## Branching : 

* git branch branch-name : Create a new branch -> ex. git branch feature-login

* git checkout branch-name : Switch to a branch -> ex. git checkout branch-name

* git checkout -b branch-name : Create + switch together -> ex. git checkout -b feature-login

* git branch : View all branches

## Merging : 

* First switch to main branch : git checkout main

* Then merge: git merge branch-name -> ex. git merge feature-login

## Deleting a branch : 

* git branch -d branch-name -> ex. git branch -d feature-login

